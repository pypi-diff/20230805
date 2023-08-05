# Comparing `tmp/discord_interactive-4.0.tar.gz` & `tmp/discord_interactive-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\discord_interactive-4.0.tar", last modified: Mon Jun 29 15:12:52 2020, max compression
+gzip compressed data, was "discord_interactive-4.1.0.tar", last modified: Sat Aug  5 17:51:29 2023, max compression
```

## Comparing `discord_interactive-4.0.tar` & `discord_interactive-4.1.0.tar`

### file list

```diff
@@ -1,9 +1,18 @@
-drwxrwxrwx   0        0        0        0 2020-06-29 15:12:52.544492 discord_interactive-4.0/
--rw-rw-rw-   0        0        0     1149 2020-06-29 15:12:52.546487 discord_interactive-4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2020-06-29 15:12:52.543632 discord_interactive-4.0/discord_interactive/
--rw-rw-rw-   0        0        0       84 2020-06-29 13:26:22.117498 discord_interactive-4.0/discord_interactive/__init__.py
--rw-rw-rw-   0        0        0     6567 2020-06-29 14:16:19.736921 discord_interactive-4.0/discord_interactive/help.py
--rw-rw-rw-   0        0        0     4886 2020-06-29 13:26:22.125081 discord_interactive-4.0/discord_interactive/link.py
--rw-rw-rw-   0        0        0    12281 2020-06-29 14:32:42.888437 discord_interactive-4.0/discord_interactive/page.py
--rw-rw-rw-   0        0        0       63 2020-06-29 13:26:22.136965 discord_interactive-4.0/setup.cfg
--rw-rw-rw-   0        0        0     2025 2020-06-29 15:04:24.797277 discord_interactive-4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:51:29.596579 discord_interactive-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-05 17:51:27.000000 discord_interactive-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-08-05 17:51:29.596579 discord_interactive-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-08-05 17:51:27.000000 discord_interactive-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:51:29.596579 discord_interactive-4.1.0/discord_interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-05 17:51:27.000000 discord_interactive-4.1.0/discord_interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-08-05 17:51:27.000000 discord_interactive-4.1.0/discord_interactive/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-08-05 17:51:27.000000 discord_interactive-4.1.0/discord_interactive/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-08-05 17:51:27.000000 discord_interactive-4.1.0/discord_interactive/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 17:51:29.596579 discord_interactive-4.1.0/discord_interactive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-08-05 17:51:29.000000 discord_interactive-4.1.0/discord_interactive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-05 17:51:29.000000 discord_interactive-4.1.0/discord_interactive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 17:51:29.000000 discord_interactive-4.1.0/discord_interactive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-05 17:51:29.000000 discord_interactive-4.1.0/discord_interactive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-05 17:51:29.000000 discord_interactive-4.1.0/discord_interactive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-08-05 17:51:27.000000 discord_interactive-4.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 17:51:29.596579 discord_interactive-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-05 17:51:27.000000 discord_interactive-4.1.0/setup.py
```

### Comparing `discord_interactive-4.0/discord_interactive/link.py` & `discord_interactive-4.1.0/discord_interactive/link.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,118 +1,128 @@
-class Link:
-    """ Base class for all type of link.
-
-    Links represent branches of the help tree.
-    All links can have callbacks, and a description.
-    Links also have a list of child pages. Most of the time, we want simple link, 
-    so the link have a single child, which is displayed if the link is taken.
-    But sometimes, we want something more complex, like if the user take link1, 
-    ans user is a specific role, we will display a different page. That's why
-    links can have several child pages. 
-    By default, if callbacks does not change this behavior, the first child of 
-    the list is selected. 
-
-    Attributes:
-        pages (list of Page): List of pages associated to this link.
-        description (str): Description of this link, to explain to user the 
-            effect of this link.
-        callbacks (list): List of functions to call when taking this link.
-        path (int): Which child page will be displayed. Default to 0 (the first
-            Page of the list).
-    """
-    def __init__(self, pages, description=None, callbacks=[]):
-        """ Link constructor
-
-        Create a Link with a list of child pages, a description, and 
-        callbacks optionally.
-
-        Args:
-            pages (list of Page or Page): List of pages associated to this link.
-            description (str, optional): Description of this link, to explain to 
-                user the effect of this link. Defaults to `None`.
-            callbacks (list, optional): List of functions to call when taking 
-                this link. Defaults to empty list.
-        """
-        # Normalize input
-        if type(pages) == list:
-            self.pages = pages
-        else:
-            self.pages = [pages]
-        if type(callbacks) == list:
-            self.callbacks = callbacks
-        else:
-            self.callbacks = [callbacks]
-
-        self.description = description
-        self.path = 0
-
-    def page(self):
-        """
-        This method is called by the Help, after calling the callbacks.
-        So the path was updated (or not) to select the right page, and we should 
-        return the appropriate page.
-
-        Returns:
-            Page: The page selected by callbacks (or default choice).
-        """
-        return self.pages[self.path]
-
-class ReactLink(Link):
-    """ Class for link using reaction to naviguate to next page.
-
-    Attributes:
-        reaction (str): Reaction needed by this link to display the page.
-    """
-    def __init__(self, reaction, pages, description=None, callbacks=[]):
-        """ ReactLink constructor
-
-        Create a ReactLink to other pages, with a reaction, and a possibly a 
-        description, as well as callbacks.
-
-        Args:
-            reaction (str): Reaction needed by this link to display the page.
-            pages (list of Page or Page): Page to display when this link is used.
-            description (str, optional): Description of this link, to explain to 
-                user the effect of this link. Defaults to `None`.
-            callbacks (list, optional): List of functions to call when taking 
-                this link. Defaults to empty list.
-        """
-        super(ReactLink, self).__init__(pages, description, callbacks)
-        self.reaction = reaction
-
-        # We need to update the description of this link to add the reaction
-        if self.description is not None:
-            self.description = self.reaction + ' ' + self.description
-
-class MsgLink(Link):
-    """ Class for link using message to naviguate to next page.
-    """
-    def __init__(self, pages, description=None, callbacks=[]):
-        """ MsgLink constructor
-
-        Create a MsgLink with a list of child pages, a description, and 
-        callbacks optionally.
-
-        Args:
-            pages (list of Page or Page): List of pages associated to this link.
-            description (str, optional): Description of this link, to explain to 
-                user the effect of this link. Defaults to `None`.
-            callbacks (list, optional): List of functions to call when taking 
-                this link. Defaults to empty list.
-        """
-        super(MsgLink, self).__init__(pages, description, callbacks)
-
-class RootLink(Link):
-    """ Class for the first link of the help tree.
-    """
-    def __init__(self, pages, callbacks=[]):
-        """ RootLink constructor
-
-        RootLink is like any other links (callbacks included), but there is no 
-        description.
-
-        Args:
-            pages (list of Page or Page): List of pages associated to this link.
-            callbacks (list, optional): List of functions to call when taking 
-                this link. Defaults to empty list.
-        """
-        super(RootLink, self).__init__(pages, callbacks=callbacks)
+"""Module containing the definition of the `Link` classes. These classes are
+not public-facing, they are used only internally.
+User can create links using the `link()` method in the `Page` class.
+"""
+
+
+class Link:
+    """Base class for all type of link.
+
+    Links represent branches of the help tree.
+    All links can have callbacks, and a description.
+    Links also have a list of child pages. Most of the time, we want simple link,
+    so the link have a single child, which is displayed if the link is taken.
+    But sometimes, we want something more complex, like if the user take link1,
+    ans user is a specific role, we will display a different page. That's why
+    links can have several child pages.
+    By default, if callbacks does not change this behavior, the first child of
+    the list is selected.
+
+    Attributes:
+        pages (list of Page): List of pages associated to this link.
+        description (str): Description of this link, to explain to user the
+            effect of this link.
+        callbacks (list): List of functions to call when taking this link.
+        path (int): Which child page will be displayed. Default to 0 (the first
+            Page of the list).
+    """
+
+    def __init__(self, pages, description=None, callbacks=[]):
+        """Link constructor.
+
+        Create a Link with a list of child pages, a description, and
+        callbacks optionally.
+
+        Args:
+            pages (list of Page or Page): List of pages associated to this link.
+            description (str, optional): Description of this link, to explain to
+                user the effect of this link. Defaults to `None`.
+            callbacks (list, optional): List of functions to call when taking
+                this link. Defaults to empty list.
+        """
+        # Normalize input
+        if type(pages) == list:
+            self.pages = pages
+        else:
+            self.pages = [pages]
+        if type(callbacks) == list:
+            self.callbacks = callbacks
+        else:
+            self.callbacks = [callbacks]
+
+        self.description = description
+        self.path = 0
+
+    def page(self):
+        """This method is called by the Help, after calling the callbacks.
+        So the path was updated (or not) to select the right page, and we should
+        return the appropriate page.
+
+        Returns:
+            Page: The page selected by callbacks (or default choice).
+        """
+        return self.pages[self.path]
+
+
+class ReactLink(Link):
+    """Class for link using reaction to naviguate to next page.
+
+    Attributes:
+        reaction (str): Reaction needed by this link to display the page.
+    """
+
+    def __init__(self, reaction, pages, description=None, callbacks=[]):
+        """ReactLink constructor.
+
+        Create a ReactLink to other pages, with a reaction, and a possibly a
+        description, as well as callbacks.
+
+        Args:
+            reaction (str): Reaction needed by this link to display the page.
+            pages (list of Page or Page): Page to display when this link is used.
+            description (str, optional): Description of this link, to explain to
+                user the effect of this link. Defaults to `None`.
+            callbacks (list, optional): List of functions to call when taking
+                this link. Defaults to empty list.
+        """
+        super(ReactLink, self).__init__(pages, description, callbacks)
+        self.reaction = reaction
+
+        # We need to update the description of this link to add the reaction
+        if self.description is not None:
+            self.description = self.reaction + " " + self.description
+
+
+class MsgLink(Link):
+    """Class for link using message to naviguate to next page."""
+
+    def __init__(self, pages, description=None, callbacks=[]):
+        """MsgLink constructor.
+
+        Create a MsgLink with a list of child pages, a description, and
+        callbacks optionally.
+
+        Args:
+            pages (list of Page or Page): List of pages associated to this link.
+            description (str, optional): Description of this link, to explain to
+                user the effect of this link. Defaults to `None`.
+            callbacks (list, optional): List of functions to call when taking
+                this link. Defaults to empty list.
+        """
+        super(MsgLink, self).__init__(pages, description, callbacks)
+
+
+class RootLink(Link):
+    """Class for the first link of the help tree."""
+
+    def __init__(self, pages, callbacks=[]):
+        """RootLink constructor.
+
+        RootLink is like any other links (callbacks included), but there is no
+        description.
+
+        Args:
+            pages (list of Page or Page): List of pages associated to this link.
+            callbacks (list, optional): List of functions to call when taking
+                this link. Defaults to empty list.
+        """
+        super(RootLink, self).__init__(pages, callbacks=callbacks)
```

### Comparing `discord_interactive-4.0/discord_interactive/page.py` & `discord_interactive-4.1.0/discord_interactive/page.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,298 +1,311 @@
-from enum import Enum, auto
-
-import discord
-
-from discord_interactive.link import ReactLink, MsgLink
-
-DEFAULT_PARENT_REACT = '🔙'
-DEFAULT_ROOT_REACT = '🔝'
-DEFAULT_LINK_REACTS = ['1⃣', '2⃣', '3⃣', '4⃣', '5⃣', '6⃣', '7⃣', '8⃣', '9⃣']
-
-
-class PageType(Enum):
-    """ Existing type of page. The type of a page define how this page will be
-    displayed.
-    """
-    MESSAGE = auto()
-    EMBED = auto()
-
-
-class Page:
-    """ Class representing a page of the help.
-
-    This class represents a page of the help. A page is displayed to the user, 
-    and the user can naviguate through pages using reaction or messages. 
-    A page have several attributes : a message, and a map of linked pages, 
-    based on reaction of the user.
-
-    Attributes:
-        msg (str): Message to display to the user when displaying the page.
-        links (list of Links): List of Links associated to this page.
-        msg_link (MsgLink): MsgLink if there is one. It's not part of the links
-            list because there can be only 1 msg link per page.
-        parent (Link): Link to the parent page.
-        root (Link): Link to the root page.
-        sep (str): String used to separate the message and the links description
-            (for display).
-        links_sep (str): String used to separate the links description (between
-            each of them) (for display).
-        type (PageType): Type of the page. Can be `PageType.MESSAGE` or
-            `PageType.EMBED`.
-    """
-
-    def __init__(self, msg='', sep='\n\n', links_sep='\n', embed=True,
-                 **embed_kwargs):
-        """ Page constructor
-
-        Constructor of the class Page. Create a Page with a message.
-
-        Args:
-            msg (str, optional): Message to display to the user when displaying 
-                the page.
-            sep (str, optional): String used to separate the message and the 
-                links description (for display). Defaults to `\n\n`.
-            links_sep (str, optional): String used to separate the links 
-                description (between each of them) (for display). Defaults to 
-                `\n`.
-            embed (bool, optional): If set to `True`, create a page of type
-                `PageType.EMBED`, if `False` the page type is
-                `PageType.MESSAGE`. Defaults to `True`.
-            embed_kwargs (dict): Others keywords arguments, used to initialize
-                the `Embed` for display. Only used if the type of the page is
-                `PageType.EMBED`.
-        """
-        self.msg = msg
-        self.links = []
-        self.msg_link = None
-        self.parent = None
-        self.root = None
-        self.sep = sep
-        self.links_sep = links_sep
-        self.type = PageType.EMBED if embed else PageType.MESSAGE
-        self.embed_kwargs = embed_kwargs
-
-    ####################### Construction of the Tree ###########################
-
-    def link(self, pages, reaction=None, description=None, callbacks=[], 
-             user_input=False, is_parent=True, 
-             parent_reaction=DEFAULT_PARENT_REACT):
-        """ Page linker with reactions.
-
-        Link a page to other pages by creating a link with reaction.
-
-        Args:
-            pages (list of Page or Page): List of pages associated to this link.
-            reaction (str, optional): Reaction needed to go through the link. 
-                If None is given, use a default reaction. Defaults to `None`.
-            description (str, optional): Description of the link, to explain to 
-                user the effect of this link. Defaults to `None`.
-            callbacks (list, optional): List of functions to call when taking 
-                this link. Defaults to empty list.
-            user_input (bool, optional): Boolean indicating if this is a MsgLink 
-                or not. Defaults to `False`.
-            is_parent (bool, optional): Boolean indicating if the currentpage 
-                should be represented as the parent of the pages linked. 
-                Defaults to `True`.
-            parent_reaction (str or list of str, optional): Reaction to use for 
-                the child to come back to its parent (current page). If a list
-                is given, each reaction is associated to one page of the list
-                of pages given. Defaults to `🔙`.
-
-        Throws:
-            IndexError: Only the 9 first links are provided with default 
-                reactions (digit 1 ~ 9). If you try to create another link with 
-                default reaction, this Exception will be thrown. 
-            ValueError: The number of parent reaction given does not correspond
-                to the number of child pages.
-        """
-        # Create the appropriate link
-        if user_input:        # Create a MsgLink
-            self.msg_link = MsgLink(pages, description, callbacks)
-        else:                           # Create a ReactLink
-            # First, retrieve the default reaction if none was given
-            if reaction is None:
-                reaction = DEFAULT_LINK_REACTS[len(self.links)]
-
-            # Then create a ReactLink
-            l = ReactLink(reaction, pages, description, callbacks)
-
-            # And link it to this page
-            self.links.append(l)
-
-        # Create the parent links
-        if is_parent:
-            self.parent_of(pages, parent_reaction)
-
-    def parent_of(self, pages, parent_reaction=DEFAULT_PARENT_REACT):
-        """ Parent Page linker.
-
-        Link a list of pages the current page as a parent.
-
-        Args:
-            pages (list of Page or Page): List of pages to associate the current
-                page as a parent.
-            parent_reaction (str or list of str, optional): Reaction to use for 
-                the child to come back to its parent (current page). If a list
-                is given, each reaction is associated to one page of the list
-                of pages given. Defaults to `🔙`.
-
-        Throws:
-            ValueError: The number of parent reaction given does not correspond
-                to the number of child pages.
-        """
-        # Normalize list of pages
-        if type(pages) != list:
-            pages = [pages]
-
-        if type(parent_reaction) == list:
-            if len(pages) != len(parent_reaction):
-                raise ValueError("You gave a list of reaction for the parent " \
-                    "page, but the number of pages given are not matching this" \
-                    " list ({} pages, but {} reactions)".format(len(pages), 
-                    len(parent_reaction)))
-        else:   # Normalize list of reaction
-            parent_reaction = [parent_reaction] * len(pages)
-
-        # Assign to each page this page as parent with the right reaction
-        for p, r in zip(pages, parent_reaction):
-            # First, create the parent link
-            p_link = ReactLink(r, self)
-
-            # Then associate this link to the page
-            p.parent = p_link
-
-    def root_of(self, pages, root_reaction=DEFAULT_ROOT_REACT):
-        """ Root Page linker.
-
-        Link a list of pages the current page as root.
-
-        Args:
-            pages (list of Page or Page): List of pages to associate the current
-                page as root.
-            root_reaction (str or list of str, optional): Reaction to use for 
-                the pages to come back to the root (current page). If a list
-                is given, each reaction is associated to one page of the list
-                of pages given. Defaults to `🔝`.
-
-        Throws:
-            ValueError: The number of root reaction given does not correspond
-                to the number of pages given.
-        """
-        # Normalize list of pages
-        if type(pages) != list:
-            pages = [pages]
-
-        if type(root_reaction) == list:
-            if len(pages) != len(root_reaction):
-                raise ValueError("You gave a list of reaction for the root " \
-                    "page, but the number of pages given are not matching this" \
-                    " list ({} pages, but {} reactions)".format(len(pages), 
-                    len(root_reaction)))
-        else:   # Normalize list of reaction
-            root_reaction = [root_reaction] * len(pages)
-
-        # Assign to each page this page as parent with the right reaction
-        for p, r in zip(pages, root_reaction):
-            # First, create the parent link
-            r_link = ReactLink(r, self)
-
-            # Then associate this link to the page
-            p.root = r_link
-
-    ######################## Display of the Tree ###############################
-
-    def get_message(self):
-        """
-        This method is called by the Help if the page is a `PageType.MESSAGE`.
-        It returns the formatted content of the Page as a string.
-        This will display the main message of the Page, as well as the message
-        describing each Link of the Page.
-        This method simply construct the string to send to the channel.
-
-        Returns:
-            str: Content to display to user.
-        """
-        content = self.msg
-        content += self.sep
-        content += self.links_sep.join([l.description for l in self.links if \
-            l.description is not None])
-        if self.msg_link is not None and self.msg_link.description is not None:
-            content += self.links_sep + self.msg_link.description
-        return content
-
-    def get_embed(self):
-        """
-        This method is called by the Help if the page is a `PageType.EMBED`.
-        It returns an `Embed` object, representing the formatted page.
-        This will display the main message of the Page, as well as the message
-        describing each Link of the Page.
-
-        Returns:
-            Embed: Embed to display to user.
-        """
-        return discord.Embed(description=self.get_message(), **self.embed_kwargs)
-
-    def reactions(self):
-        """
-        This method is called by the Help, to retrieve the list of reactions 
-        that the user can use to interact with the help.
-
-        Returns:
-            list of str: List of reactions (str) that the user can use for this
-                page.
-        """
-        return [l.reaction for l in self._all_links()]
-
-    def need_user_input(self):
-        """ Method to know if the Help display needs to wait for the user to 
-        input something. 
-
-        If the page contains a MsgLink, then the helper needs to wait the user 
-        to input something.
-
-        Returns:
-            bool: True if there is MsgLink, False otherwise.
-        """
-        return self.msg_link is not None
-
-    def next_link(self, reaction=None):
-        """Accessing the next Link.
-
-        This function access the next Link based on the reaction given. If the 
-        reaction is `None`, retrieve the MsgLink. If the reaction is not valid 
-        (no link associated to this reaction), `None` is returned.
-
-        Args:
-            reaction (str, optional): Reaction chosen by the user, representing 
-                a Link. If `None`, the link returned is MsgLink. Default to None. 
-
-        Returns:
-            Link or None: The next link to display, based on the reaction of 
-                the user, or `None` if the choice of the user is not valid.
-        """
-        if reaction is None:
-            return self.msg_link
-
-        next_link = None
-        for l in self._all_links():
-            if l.reaction == reaction:
-                next_link = l
-        return next_link
-
-    ############################## Private #####################################
-
-    def _all_links(self):
-        """ Private function
-
-        Return a list of available ReactLink for this page.
-
-        Returns:
-            list of ReactLink: All links.
-        """
-        all_links = self.links
-        if self.parent is not None:
-            all_links += [self.parent]
-        if self.root is not None:
-            all_links += [self.root]
-        return all_links
-
+"""Module containing the definition of the `Page` class, which is the main
+class to define the pages of your interactive help for your Discord bot.
+"""
+
+
+from enum import Enum, auto
+
+import discord
+
+from discord_interactive.link import MsgLink, ReactLink
+
+
+DEFAULT_PARENT_REACT = "🔙"
+DEFAULT_ROOT_REACT = "🔝"
+DEFAULT_LINK_REACTS = ["1⃣", "2⃣", "3⃣", "4⃣", "5⃣", "6⃣", "7⃣", "8⃣", "9⃣"]
+
+
+class PageType(Enum):
+    """Existing type of page. The type of a page define how this page will be
+    displayed.
+    """
+
+    MESSAGE = auto()
+    EMBED = auto()
+
+
+class Page:
+    """Class representing a page of the help.
+
+    This class represents a page of the help. A page is displayed to the user,
+    and the user can naviguate through pages using reaction or messages.
+    A page have several attributes : a message, and a map of linked pages,
+    based on reaction of the user.
+
+    Attributes:
+        msg (str): Message to display to the user when displaying the page.
+        links (list of Links): List of Links associated to this page.
+        msg_link (MsgLink): MsgLink if there is one. It's not part of the links
+            list because there can be only 1 msg link per page.
+        parent (Link): Link to the parent page.
+        root (Link): Link to the root page.
+        sep (str): String used to separate the message and the links description
+            (for display).
+        links_sep (str): String used to separate the links description (between
+            each of them) (for display).
+        type (PageType): Type of the page. Can be `PageType.MESSAGE` or
+            `PageType.EMBED`.
+        embed_kwargs (dict): Others keywords arguments, used to initialize
+            the `Embed` for display. Only used if the type of the page is
+            `PageType.EMBED`.
+    """
+
+    def __init__(self, msg="", sep="\n\n", links_sep="\n", embed=True, **embed_kwargs):
+        r"""Page constructor.
+
+        Constructor of the class Page. Create a Page with a message.
+
+        Args:
+            msg (str, optional): Message to display to the user when displaying
+                the page.
+            sep (str, optional): String used to separate the message and the
+                links description (for display). Defaults to `\n\n`.
+            links_sep (str, optional): String used to separate the links
+                description (between each of them) (for display). Defaults to
+                `\n`.
+            embed (bool, optional): If set to `True`, create a page of type
+                `PageType.EMBED`, if `False` the page type is
+                `PageType.MESSAGE`. Defaults to `True`.
+            embed_kwargs (dict): Others keywords arguments, used to initialize
+                the `Embed` for display. Only used if the type of the page is
+                `PageType.EMBED`.
+        """
+        self.msg = msg
+        self.links = []
+        self.msg_link = None
+        self.parent = None
+        self.root = None
+        self.sep = sep
+        self.links_sep = links_sep
+        self.type = PageType.EMBED if embed else PageType.MESSAGE
+        self.embed_kwargs = embed_kwargs
+
+    ####################### Construction of the Tree ###########################
+
+    def link(
+        self,
+        pages,
+        reaction=None,
+        description=None,
+        callbacks=[],
+        user_input=False,
+        is_parent=True,
+        parent_reaction=DEFAULT_PARENT_REACT,
+    ):
+        """Page linker with reactions.
+
+        Link a page to other pages by creating a link with reaction.
+
+        Args:
+            pages (list of Page or Page): List of pages associated to this link.
+            reaction (str, optional): Reaction needed to go through the link.
+                If None is given, use a default reaction. Defaults to `None`.
+            description (str, optional): Description of the link, to explain to
+                user the effect of this link. Defaults to `None`.
+            callbacks (list, optional): List of functions to call when taking
+                this link. Defaults to empty list.
+            user_input (bool, optional): Boolean indicating if this is a MsgLink
+                or not. Defaults to `False`.
+            is_parent (bool, optional): Boolean indicating if the currentpage
+                should be represented as the parent of the pages linked.
+                Defaults to `True`.
+            parent_reaction (str or list of str, optional): Reaction to use for
+                the child to come back to its parent (current page). If a list
+                is given, each reaction is associated to one page of the list
+                of pages given. Defaults to `🔙`.
+
+        Throws:
+            IndexError: Only the 9 first links are provided with default
+                reactions (digit 1 ~ 9). If you try to create another link with
+                default reaction, this Exception will be thrown.
+            ValueError: The number of parent reaction given does not correspond
+                to the number of child pages.
+        """
+        # Create the appropriate link
+        if user_input:  # Create a MsgLink
+            self.msg_link = MsgLink(pages, description, callbacks)
+        else:  # Create a ReactLink
+            # First, retrieve the default reaction if none was given
+            if reaction is None:
+                reaction = DEFAULT_LINK_REACTS[len(self.links)]
+
+            # Then create a ReactLink
+            link = ReactLink(reaction, pages, description, callbacks)
+
+            # And link it to this page
+            self.links.append(link)
+
+        # Create the parent links
+        if is_parent:
+            self.parent_of(pages, parent_reaction)
+
+    def parent_of(self, pages, parent_reaction=DEFAULT_PARENT_REACT):
+        """Parent Page linker.
+
+        Link a list of pages the current page as a parent.
+
+        Args:
+            pages (list of Page or Page): List of pages to associate the current
+                page as a parent.
+            parent_reaction (str or list of str, optional): Reaction to use for
+                the child to come back to its parent (current page). If a list
+                is given, each reaction is associated to one page of the list
+                of pages given. Defaults to `🔙`.
+
+        Throws:
+            ValueError: The number of parent reaction given does not correspond
+                to the number of child pages.
+        """
+        # Normalize list of pages
+        if type(pages) != list:
+            pages = [pages]
+
+        if type(parent_reaction) == list:
+            if len(pages) != len(parent_reaction):
+                raise ValueError(
+                    "You gave a list of reaction for the parent "
+                    "page, but the number of pages given are not matching this"
+                    " list ({} pages, but {} reactions)".format(len(pages), len(parent_reaction))
+                )
+        else:  # Normalize list of reaction
+            parent_reaction = [parent_reaction] * len(pages)
+
+        # Assign to each page this page as parent with the right reaction
+        for p, r in zip(pages, parent_reaction):
+            # First, create the parent link
+            p_link = ReactLink(r, self)
+
+            # Then associate this link to the page
+            p.parent = p_link
+
+    def root_of(self, pages, root_reaction=DEFAULT_ROOT_REACT):
+        """Root Page linker.
+
+        Link a list of pages the current page as root.
+
+        Args:
+            pages (list of Page or Page): List of pages to associate the current
+                page as root.
+            root_reaction (str or list of str, optional): Reaction to use for
+                the pages to come back to the root (current page). If a list
+                is given, each reaction is associated to one page of the list
+                of pages given. Defaults to `🔝`.
+
+        Throws:
+            ValueError: The number of root reaction given does not correspond
+                to the number of pages given.
+        """
+        # Normalize list of pages
+        if type(pages) != list:
+            pages = [pages]
+
+        if type(root_reaction) == list:
+            if len(pages) != len(root_reaction):
+                raise ValueError(
+                    "You gave a list of reaction for the root "
+                    "page, but the number of pages given are not matching this"
+                    " list ({} pages, but {} reactions)".format(len(pages), len(root_reaction))
+                )
+        else:  # Normalize list of reaction
+            root_reaction = [root_reaction] * len(pages)
+
+        # Assign to each page this page as parent with the right reaction
+        for p, r in zip(pages, root_reaction):
+            # First, create the parent link
+            r_link = ReactLink(r, self)
+
+            # Then associate this link to the page
+            p.root = r_link
+
+    ######################## Display of the Tree ###############################
+
+    def get_message(self):
+        """This method is called by the Help if the page is a `PageType.MESSAGE`.
+        It returns the formatted content of the Page as a string.
+        This will display the main message of the Page, as well as the message
+        describing each Link of the Page.
+        This method simply construct the string to send to the channel.
+
+        Returns:
+            str: Content to display to user.
+        """
+        content = self.msg
+        content += self.sep
+        content += self.links_sep.join([link.description for link in self.links if link.description is not None])
+        if self.msg_link is not None and self.msg_link.description is not None:
+            content += self.links_sep + self.msg_link.description
+        return content
+
+    def get_embed(self):
+        """This method is called by the Help if the page is a `PageType.EMBED`.
+        It returns an `Embed` object, representing the formatted page.
+        This will display the main message of the Page, as well as the message
+        describing each Link of the Page.
+
+        Returns:
+            Embed: Embed to display to user.
+        """
+        return discord.Embed(description=self.get_message(), **self.embed_kwargs)
+
+    def reactions(self):
+        """This method is called by the Help, to retrieve the list of reactions
+        that the user can use to interact with the help.
+
+        Returns:
+            list of str: List of reactions (str) that the user can use for this
+                page.
+        """
+        return [link.reaction for link in self._all_links()]
+
+    def need_user_input(self):
+        """Method to know if the Help display needs to wait for the user to
+        input something.
+
+        If the page contains a MsgLink, then the helper needs to wait the user
+        to input something.
+
+        Returns:
+            bool: True if there is MsgLink, False otherwise.
+        """
+        return self.msg_link is not None
+
+    def next_link(self, reaction=None):
+        """Accessing the next Link.
+
+        This function access the next Link based on the reaction given. If the
+        reaction is `None`, retrieve the MsgLink. If the reaction is not valid
+        (no link associated to this reaction), `None` is returned.
+
+        Args:
+            reaction (str, optional): Reaction chosen by the user, representing
+                a Link. If `None`, the link returned is MsgLink. Default to None.
+
+        Returns:
+            Link or None: The next link to display, based on the reaction of
+                the user, or `None` if the choice of the user is not valid.
+        """
+        if reaction is None:
+            return self.msg_link
+
+        next_link = None
+        for link in self._all_links():
+            if link.reaction == reaction:
+                next_link = link
+        return next_link
+
+    ############################## Private #####################################
+
+    def _all_links(self):
+        """Private function.
+
+        Return a list of available ReactLink for this page.
+
+        Returns:
+            list of ReactLink: All links.
+        """
+        all_links = self.links
+        if self.parent is not None:
+            all_links += [self.parent]
+        if self.root is not None:
+            all_links += [self.root]
+        return all_links
```

