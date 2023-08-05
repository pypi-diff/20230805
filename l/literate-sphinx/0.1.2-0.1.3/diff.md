# Comparing `tmp/literate-sphinx-0.1.2.tar.gz` & `tmp/literate-sphinx-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "literate-sphinx-0.1.2.tar", last modified: Sat Jan 21 23:40:28 2023, max compression
+gzip compressed data, was "literate-sphinx-0.1.3.tar", last modified: Sat Aug  5 00:27:39 2023, max compression
```

## Comparing `literate-sphinx-0.1.2.tar` & `literate-sphinx-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       38 2023-01-21 02:38:39.883341 literate-sphinx-0.1.2/.gitignore
--rw-r--r--   0        0        0      414 2023-01-21 02:37:00.270847 literate-sphinx-0.1.2/.gitlab-ci.yml
--rw-r--r--   0        0        0     1265 2023-01-16 21:36:06.038394 literate-sphinx-0.1.2/LICENSES/BSD-2-Clause.txt
--rw-r--r--   0        0        0      929 2023-01-21 02:38:08.119183 literate-sphinx-0.1.2/Makefile
--rw-r--r--   0        0        0    27639 2023-01-21 23:16:09.771488 literate-sphinx-0.1.2/code.md
--rw-r--r--   0        0        0     1326 2023-01-21 03:22:55.399074 literate-sphinx-0.1.2/conf.py
--rw-r--r--   0        0        0     5088 2023-01-21 02:58:17.064050 literate-sphinx-0.1.2/index.md
--rw-r--r--   0        0        0    14360 2023-01-21 23:21:52.866052 literate-sphinx-0.1.2/literate_sphinx.py
--rw-r--r--   0        0        0      800 2023-01-16 04:35:00.299706 literate-sphinx-0.1.2/make.bat
--rw-r--r--   0        0        0      807 2023-01-20 00:26:58.467104 literate-sphinx-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      651 2023-01-18 20:10:17.127898 literate-sphinx-0.1.2/requirements.txt
--rw-r--r--   0        0        0     5796 1970-01-01 00:00:00.000000 literate-sphinx-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       38 2023-01-21 02:38:39.883341 literate-sphinx-0.1.3/.gitignore
+-rw-r--r--   0        0        0      603 2023-07-21 22:51:04.407838 literate-sphinx-0.1.3/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1265 2023-01-16 21:36:06.038394 literate-sphinx-0.1.3/LICENSES/BSD-2-Clause.txt
+-rw-r--r--   0        0        0      929 2023-01-21 02:38:08.119183 literate-sphinx-0.1.3/Makefile
+-rw-r--r--   0        0        0    29985 2023-08-05 00:23:50.718955 literate-sphinx-0.1.3/code.md
+-rw-r--r--   0        0        0     1326 2023-01-21 03:22:55.399074 literate-sphinx-0.1.3/conf.py
+-rw-r--r--   0        0        0     5462 2023-07-21 02:40:32.448117 literate-sphinx-0.1.3/index.md
+-rw-r--r--   0        0        0    16319 2023-08-05 00:24:50.923774 literate-sphinx-0.1.3/literate_sphinx.py
+-rw-r--r--   0        0        0      800 2023-01-16 04:35:00.299706 literate-sphinx-0.1.3/make.bat
+-rw-r--r--   0        0        0      866 2023-07-19 03:45:05.534074 literate-sphinx-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      777 2023-07-22 02:12:16.206116 literate-sphinx-0.1.3/requirements.txt
+-rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 literate-sphinx-0.1.3/PKG-INFO
```

### Comparing `literate-sphinx-0.1.2/LICENSES/BSD-2-Clause.txt` & `literate-sphinx-0.1.3/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `literate-sphinx-0.1.2/Makefile` & `literate-sphinx-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `literate-sphinx-0.1.2/code.md` & `literate-sphinx-0.1.3/code.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,22 @@
 Here is the implementation of the extension.
 
 ## `literate-code` directive
 
 First, we define the `literate-code` directive:
 
 ```{literate-code} classes
+:padding: 2
+
 class LiterateCode(SphinxDirective):
     """Parse and mark up content of a literate code chunk.
 
     The argument is the chunk name
     """
+
     {{LiterateCode variables}}
 
     {{LiterateCode methods}}
 ```
 
 The directive takes one argument, which is required, and may contain
 whitespace.
@@ -26,18 +29,19 @@
 ```
 
 The options are as defined above.  The `directives.*` values below specify how
 the option values are validated.
 
 ```{literate-code} LiterateCode variables
 option_spec = {
-    'class': directives.class_option,
-    'file': directives.flag,
-    'lang': directives.unchanged,
-    'name': directives.unchanged,
+    "class": directives.class_option,
+    "file": directives.flag,
+    "lang": directives.unchanged,
+    "padding": directives.unchanged,
+    "name": directives.unchanged,
 }
 ```
 
 Obviously, code chunks need to have content.
 
 ```{literate-code} LiterateCode variables
 has_content = True
@@ -45,15 +49,15 @@
 
 Directives need one method: a `run` method that outputs a list of docutils
 nodes to insert into the document.  Our `run` method will have three phases:
 options processing, creating the `literal_block` to contain the code, and
 creating a `container` node around the `literal_block` to add a caption.
 
 ```{literate-code} LiterateCode methods
-def run(self) -> list[nodes.Node]:
+def run(self) -> list[nodes.Element]:
     {{process literate-code options}}
 
     {{create literal_block}}
 
     {{create container node}}
 ```
 
@@ -65,53 +69,78 @@
 ```
 
 Next, we determine the language used for syntax highlighting.  If a `:lang:`
 option is given, we will use that value.  Otherwise, we use the
 `highlight_language` config option.
 
 ```{literate-code} process literate-code options
-language = options['lang'] if 'lang' in options else \
-    self.env.temp_data.get('highlight_language', self.config.highlight_language)
+language = (
+    options["lang"]
+    if "lang" in options
+    else self.env.temp_data.get(
+        "highlight_language", self.config.highlight_language
+    )
+)
 ```
 
 If the `file` option is given, then the chunk represents a file.
 
 ```{literate-code} process literate-code options
-is_file = 'file' in options
+is_file = "file" in options
 ```
 
 The chunk name is the arguments given to the directive.
 
 ```{literate-code} process literate-code options
 chunk_name = self.arguments[0]
 ```
 
+When there are multiple chunks with the same name, they will be written out it
+sequence.  The `padding` option indicates whether there should be blank lines
+between this chunk and the *previous* chunk of the same name, and how many
+blanks lines there should be.  If the option is given without an argument, then
+one line is used.  If the option is not given, then the `default_chunk_padding`
+option is used.
+
+```{literate-code} process literate-code options
+if "padding" in options:
+    if options["padding"] == "":
+        padding = 1
+    else:
+        padding = int(options["padding"])
+else:
+    padding = self.config.default_chunk_padding
+```
+
 The code is the contents given to the directive.  The contents are given as a
 list of lines, so we join them together with `\n`.
 
 ```{literate-code} process literate-code options
-code = '\n'.join(self.content)
+code = "\n".join(self.content)
 ```
 
 The code will be displayed in a `literal_block` (a mono-spaced block), and we
 will add some attributes to store the options that were given.  The
-`code-chunk-name` and `code-chunk-is-file` attributes will be used for
-tangling.  The `language` attribute is used for syntax highlighting, and the
-`classes` attribute is used for rendering the document.
+`code-chunk-name`, `code-chunk-is-file`, and `code-chunk-padding` attributes
+will be used for tangling.  The `language` attribute is used for syntax
+highlighting, and the `classes` attribute is used for rendering the document.
 
 ```{literate-code} create literal_block
 literal_node = nodes.literal_block(code, code)
 
-literal_node['code-chunk-name'] = chunk_name
+literal_node["code-chunk-name"] = chunk_name
 if is_file:
-    literal_node['code-chunk-is-file'] = True
-literal_node['language'] = language
-literal_node['classes'].append('literate-code') # allow special styling of literate blocks
-if 'classes' in options:
-    literal_node['classes'] += options['classes']
+    literal_node["code-chunk-is-file"] = True
+literal_node["code-chunk-padding"] = padding
+literal_node["language"] = language
+literal_node["classes"].append(
+    "literate-code"
+)  # allow special styling of literate blocks
+if "classes" in options:
+    literal_node["classes"] += options["classes"]
 ```
 
 We also call `set_source_info` from the parent class to set the source file and
 line number for the node.
 
 ```{literate-code} create literal_block
 self.set_source_info(literal_node)
@@ -121,27 +150,28 @@
 `caption`.  We will use the code chunk name, followed by a `:`, as the caption,
 so that readers can see the name.  If the code chunk is a file, we make the
 caption monospaced.  The following code is based on the source code of
 `sphinx.directives.code.container_wrapper`.
 
 ```{literate-code} create container node
 container_node = nodes.container(
-    '', literal_block=True,
-    classes=['literal-block-wrapper', 'literate-code-wrapper']
+    "",
+    literal_block=True,
+    classes=["literal-block-wrapper", "literate-code-wrapper"],
 )
 
 if is_file:
     caption_node = nodes.caption(
-        chunk_name + ':',
-        '',
+        chunk_name + ":",
+        "",
         nodes.literal(chunk_name, chunk_name),
-        nodes.Text(':'),
+        nodes.Text(":"),
     )
 else:
-    caption_node = nodes.caption(chunk_name + ':', chunk_name + ':')
+    caption_node = nodes.caption(chunk_name + ":", chunk_name + ":")
 
 self.set_source_info(caption_node)
 
 container_node += caption_node
 container_node += literal_node
 ```
 
@@ -161,51 +191,53 @@
 
 ## `tangle` builder
 
 We now create a Sphinx `Builder` to "tangle" the document, that is, extract the
 code chunks and produce the computer-readable source files.
 
 ```{literate-code} classes
+:padding: 2
+
 class TangleBuilder(Builder):
     {{TangleBuilder variables}}
 
     {{TangleBuilder methods}}
 ```
 
 We give our builder the name `tangle`, so the tangling can be done by running
 `make tangle`, or using `sphinx-build -b tangle ...`.
 
 ```{literate-code} TangleBuilder variables
-name = 'tangle'
+name = "tangle"
 ```
 
 When the builder completes, we will tell the user where the tangled files can
 be found.
 
 ```{literate-code} TangleBuilder variables
-epilog = 'The tangled files are in %(outdir)s.'
+epilog = "The tangled files are in %(outdir)s."
 ```
 
 Builders need to implement several methods, some of which do not really apply
 to us.
 
 Since the output files don't correspond to input files, we tell Sphinx to read
 all the inputs.
 
 ```{literate-code} TangleBuilder methods
 def get_outdated_docs(self) -> str:
-    return 'all documents'
+    return "all documents"
 ```
 
 We don't need to worry about generating URIs for our documents, since we will
 not be creating references, so we just return an empty string.
 
 ```{literate-code} TangleBuilder methods
-def get_target_uri(self, docname: str, typ: str = None) -> str:
-    return ''
+def get_target_uri(self, docname: str, typ: Optional[str] = None) -> str:
+    return ""
 ```
 
 Now, we need a method that will give us the entire document as a single tree.
 This function is taken from `sphinx.builders.singlehtml.SingleFileHTMLBuilder`.
 
 ```{literate-code} TangleBuilder methods
 def assemble_doctree(self) -> nodes.document:
@@ -221,16 +253,18 @@
 the code chunks.  We will record the chunks with their names, and if they
 represent files, record their names in a list.  After all the chunks are
 recorded, we will go through the list of files and write the files, expanding
 the code chunk references as necessary.
 
 ```{literate-code} TangleBuilder methods
 def write(self, *ignored: Any) -> None:
-    chunks = {} # dict of chunk name to list of chunks defined by that name
-    files = [] # the list of files
+    chunks: dict[
+        str, list[nodes.Element]
+    ] = {}  # dict of chunk name to list of chunks defined by that name
+    files: list[str] = []  # the list of files
 
     doctree = self.assemble_doctree()
 
     {{find code chunks in document}}
 
     {{write files}}
 ```
@@ -238,18 +272,18 @@
 To look for code chunks, we walk the document tree, and find any
 `literal_block` nodes that have a `code-chunk-name` attribute.  If the node
 also has a `code-chunk-is-file` attribute, then we record the chunk name in the
 `files` list.
 
 ```{literate-code} find code chunks in document
 for node in doctree.findall(nodes.literal_block):
-    if 'code-chunk-name' in node:
-        name = node['code-chunk-name']
+    if "code-chunk-name" in node:
+        name = node["code-chunk-name"]
         chunks.setdefault(name, []).append(node)
-        if 'code-chunk-is-file' in node:
+        if "code-chunk-is-file" in node:
             files.append(name)
 ```
 
 Before we write the part of the function that will write out the files, we need
 two extra pieces.  The first is a class that we will use for abstracting out
 the writing of a file.  We will create a base version here, and extend the
 class when for the [annotated tangler](#annotated-tangling).  This will allow
@@ -266,61 +300,70 @@
 writer class.
 
 The function will be passed the writer object, the line to write, the
 dictionary of chunks, the prefix and suffix to add to the line, and the left
 and right delimiters used to enclose code chunk references.
 
 ```{literate-code} functions
+:padding: 2
+
 def _write_line(
-        writer: TangleWriter,
-        line: str,
-        chunks: dict[str, Any],
-        prefix: str,
-        suffix: str,
-        ldelim: str,
-        rdelim: str,
+    writer: TangleWriter,
+    line: str,
+    chunks: dict[str, Any],
+    prefix: str,
+    suffix: str,
+    ldelim: str,
+    rdelim: str,
 ) -> None:
     # check if the line contains the left and right delimiter
     s1 = line.split(ldelim, 1)
     if len(s1) == 2:
         s2 = s1[1].rsplit(rdelim, 1)
         if len(s2) == 2:
             # delimiters found, so get the chunk name
             chunk_name = s2[0].strip()
 
             # write the chunks associated with the name
             try:
                 ref_chunks = chunks[chunk_name]
             except KeyError:
                 raise ExtensionError(
-                    'Unknown chunk name: {}'.format(chunk_name),
-                    modname = __name__,
+                    f"Unknown chunk name: {chunk_name}",
+                    modname=__name__,
                 )
             writer.enter_expansion(chunk_name)
+            first = True
             for ins_chunk in ref_chunks:
-                writer.enter_chunk(ins_chunk)
+                writer.enter_chunk(ins_chunk, first)
                 for ins_line in ins_chunk.astext().splitlines():
                     # recursively call this function with each line of the
                     # referenced code chunks
                     _write_line(
                         writer,
                         ins_line,
                         chunks,
                         prefix + s1[0],
                         s2[1] + suffix,
                         ldelim,
                         rdelim,
                     )
-                writer.exit_chunk()
+                writer.exit_chunk(first)
+                first = False
             writer.exit_expansion()
 
             return
 
     # delimiters not found, so just write the line
-    writer.write_line(prefix + line + suffix)
+    if not line and not suffix:
+        # if line and suffix are both blank, strip off trailing whitespace
+        # from the prefix
+        writer.write_line(prefix.rstrip())
+    else:
+        writer.write_line(prefix + line + suffix)
 ```
 
 Now we define our writer class.  In addition to writing files, we will also use
 our writer class to handle some bookkeeping.  This bookkeeping could be done in
 our writer function, which may be better in terms of making our class only
 responsible for one thing, but putting it in the class avoids needing to pass
 more parameters into the writer function.
@@ -344,59 +387,57 @@
 the output directory, the `unused` set created by the builder, and a suffix to
 add to the file name.  For normal tangling, this will be empty, but it will be
 used with the annotated tangling defined later on.  The constructor will do
 some basic sanity checking on the file name, to ensure that it won't overwrite
 files outside of the output directory, and then create the file to be written.
 
 ```{literate-code} classes
+:padding: 2
+
 class TangleWriter:
     {{TangleWriter methods}}
 ```
 
 ```{literate-code} TangleWriter methods
 def __init__(
-        self,
-        filename: str,
-        outdir: str,
-        unused: set[str],
-        filename_suffix: str = ''
+    self, filename: str, outdir: str, unused: set[str], filename_suffix: str = ""
 ):
     self.unused = unused
-    self.path = []
+    self.path: list[str] = []
 
     # some basic sanity checking for the file name
-    if '..' in filename or os.path.isabs(filename):
+    if ".." in filename or os.path.isabs(filename):
         raise ExtensionError(
-            "Chunk name is invalid file name: {}".format(filename),
+            f"Chunk name is invalid file name: {filename}",
             modname=__name__,
         )
     # determine the full path, and make sure the directory exists before
     # creating the file
     fullpath = os.path.join(outdir, filename)
     dirname = os.path.dirname(fullpath)
     if dirname:
         os.makedirs(dirname, exist_ok=True)
 
     self.filename = filename
 
-    self.f = open(fullpath + filename_suffix, 'w')
+    self.f = open(fullpath + filename_suffix, "w")
 ```
 
 We need to close the file once we are done, so we define a method to do that.
 
 ```{literate-code} TangleWriter methods
 def close(self) -> None:
     self.f.close()
 ```
 
 And we create the `__enter__` and `__exit__` methods needed to use our class
 with the `with` statement.
 
 ```{literate-code} TangleWriter methods
-def __enter__(self) -> 'TangleWriter':
+def __enter__(self) -> "TangleWriter":
     return self
 
 def __exit__(self, *ignored: Any) -> None:
     self.close()
 ```
 
 The rest of the class is fairly straightforward.  As mentioned above, we need
@@ -405,43 +446,45 @@
 chunk reference and when we're done expanding it (here, we just need to perform
 our bookkeeping tasks), and to let it know when we're about to start processing
 a new code chunk and when we're done processing it (here, we don't need to do
 anything).
 
 ```{literate-code} TangleWriter methods
 def write_line(self, line: str) -> None:
-    self.f.write(line + '\n')
+    self.f.write(line + "\n")
 
 def enter_expansion(self, chunk_name: str, is_file: bool = False) -> None:
     # update bookeeping variables
     self.unused.discard(chunk_name)
     if chunk_name in self.path:
         self.path.append(chunk_name)
         raise ExtensionError(
-            'Loop found in chunks: {}'.format(' -> '.join(self.path)),
-            modname = __name__,
+            "Loop found in chunks: {}".format(" -> ".join(self.path)),
+            modname=__name__,
         )
     self.path.append(chunk_name)
 
 def exit_expansion(self) -> None:
     self.path.pop()
 
-def enter_chunk(self, chunk_node: nodes.Node) -> None:
-    pass
+def enter_chunk(self, chunk_node: nodes.Element, first: bool) -> None:
+    if not first:
+        for i in range(0, chunk_node["code-chunk-padding"]):
+            self.f.write("\n")
 
-def exit_chunk(self) -> None:
+def exit_chunk(self, first: bool) -> None:
     pass
 ```
 
 We add a method to our builder that returns an instance of our writer class.
 For other types of tangling, we can override this method to return a different
 type of writer.
 
 ```{literate-code} TangleBuilder methods
-def writer(self, filename: str, unused: set[str]) -> 'TangleWriter':
+def writer(self, filename: str, unused: set[str]) -> "TangleWriter":
     return TangleWriter(filename, self.outdir, unused)
 ```
 
 We can now finish off our `write` function.  For each output file, we create
 the file, look up the code chunks for the file, get the contents of each chunk,
 split into lines, and use our function above to write the lines.
 
@@ -451,31 +494,34 @@
 
 # get all the chunk names; initially, all chunks are unused
 unused = {name for name in chunks}
 
 for filename in files:
     with self.writer(filename, unused) as writer:
         writer.enter_expansion(filename, True)
+        first = True
         for chunk in chunks[filename]:
-            writer.enter_chunk(chunk)
+            writer.enter_chunk(chunk, first)
             for line in chunk.astext().splitlines():
-                _write_line(writer, line, chunks, '', '', ldelim, rdelim)
-            writer.exit_chunk()
+                _write_line(writer, line, chunks, "", "", ldelim, rdelim)
+            writer.exit_chunk(first)
+            first = False
         writer.exit_expansion()
 ```
 
 After we've written all the files, we emit a warning for every unused chunk,
 giving the file name and line where the chunk is defined.
 
 ```{literate-code} write files
 for chunk_name in unused:
     for chunk in chunks[chunk_name]:
         logger.warning(
-            '{0.source}:{0.line}: Code chunk "{1}" defined but not used'
-                .format(chunk, chunk_name)
+            '{0.source}:{0.line}: Code chunk "{1}" defined but not used'.format(
+                chunk, chunk_name
+            )
         )
 ```
 
 ## Annotated tangling
 
 In literate programming, the document is intended to be viewed by people, and
 the tangled source code is meant mainly for computers.  However, some times
@@ -495,63 +541,70 @@
 modified writer, and write out a CSS file.  We will discuss the details of
 writing out the CSS file later on, but for now, we note that we will need to
 know the maximum depth of the chunks.  We will keep track of this in our
 writer, so we will pass a our writer a reference to `self` so that it can
 update the maximum depth.
 
 ```{literate-code} classes
+:padding: 2
+
 class AnnotatedTangleBuilder(TangleBuilder):
-    name = 'annotated-tangle'
+    name = "annotated-tangle"
 
     def writer(self, filename: str, unused: set[str]) -> TangleWriter:
         return AnnotatedTangleWriter(filename, self.outdir, unused, self)
 
     def write(self, *opts: Any) -> None:
         self.max_depth = 1
 
         super().write(*opts)
 
         self.write_css()
 
     {{AnnotatedTangleBuilder methods}}
 
+
 class AnnotatedTangleWriter(TangleWriter):
     {{AnnotatedTangleWriter methods}}
 ```
 
 We will write the files as HTML, so our constructor will call the parent
 constructor, giving it a `.html` suffix.  We will add line numbers to our
 output, so we initialize our line number counter.  We will also keep track of
 the nodes on the path from the root of the file to our current chunk; this will
 be used to generate a unique ID for each path, which we will explain below.
 
 ```{literate-code} AnnotatedTangleWriter methods
 def __init__(
-        self,
-        filename: str,
-        outdir: str,
-        unused: set[str],
-        builder: AnnotatedTangleBuilder,
+    self,
+    filename: str,
+    outdir: str,
+    unused: set[str],
+    builder: AnnotatedTangleBuilder,
 ):
-    super().__init__(filename, outdir, unused, '.html')
+    super().__init__(filename, outdir, unused, ".html")
     self.lineno = 1
-    self.node_path = []
+    self.node_path: list[nodes.Node] = []
     self.builder = builder
 ```
 
 Writing out a line is fairly straghtforward.  We will output a `<div>` with an
 `id` indicating the line number, allowing users to reference individual lines.
 Inside the `<div>`, we will write the line number (making it a link to that
 line, and with an appropriate class so that it can be styled separately from
 the code), and the line of code itself.  Once we're done writing
 the line, we increment the line number.
 
 ```{literate-code} AnnotatedTangleWriter methods
 def write_line(self, line: str) -> None:
-    self.f.write('<div id="L{0}"><a class="lineno" href="#L{0}">{0}</a>{1}</div>'.format(self.lineno, html.escape(line)))
+    self.f.write(
+        '<div id="L{0}"><a class="lineno" href="#L{0}">{0}</a>{1}</div>'.format(
+            self.lineno, html.escape(line)
+        )
+    )
     self.lineno = self.lineno + 1
 ```
 
 Now we need to consider how our HTML file will be structured.  For each chunk
 name that we expand, we will create a `<ul>`.  Each chunk associated with that
 name will get a `<li>` that contains the chunk name and a `<pre>` that will
 contain the code.
@@ -573,30 +626,48 @@
 write the code.  When we exit the chunk, we close the `<pre>` and the `<li>`.
 
 We also ensure that we call the super-class implementations of the functions.
 They currently don't do anything, but we will do that in case they do something
 in the future.
 
 ```{literate-code} AnnotatedTangleWriter methods
-def enter_chunk(self, chunk_node: nodes.Node) -> None:
-    super().enter_chunk(chunk_node)
+def enter_chunk(self, chunk_node: nodes.Element, first: bool) -> None:
+    super().enter_chunk(chunk_node, first)
 
     self.node_path.append(chunk_node)
-    hash = sha256(':'.join(['{0.source}:{0.line}'.format(c) for c in self.node_path]).encode('utf-8')).hexdigest()
+    hash = sha256(
+        ":".join(["{0.source}:{0.line}".format(c) for c in self.node_path]).encode(
+            "utf-8",
+        )
+    ).hexdigest()
 
-    chunk_name = chunk_node['code-chunk-name']
-    if 'code-chunk-is-file' in chunk_node:
-        self.f.write('<li id="{}"><span class="chunkname"><code>{}</code></span><pre>'.format(hash, html.escape(chunk_name)))
+    chunk_name = chunk_node["code-chunk-name"]
+    if not first and chunk_node["code-chunk-padding"]:
+        self.f.write('<li class="gap"><pre>')
+        for i in range(0, chunk_node["code-chunk-padding"]):
+            self.f.write(
+                '<div id="L{0}"><a class="lineno" href="#L{0}">{0}</a></div>'.format(
+                    self.lineno,
+                )
+            )
+            self.lineno = self.lineno + 1
+        self.f.write("</pre></li>")
+    if "code-chunk-is-file" in chunk_node:
+        self.f.write(
+            f'<li id="{hash}"><span class="chunkname"><code>{html.escape(chunk_name)}</code></span><pre>'
+        )
     else:
-        self.f.write('<li id="{}"><span class="chunkname">{}</span><pre>'.format(hash, html.escape(chunk_name)))
+        self.f.write(
+            f'<li id="{hash}"><span class="chunkname">{html.escape(chunk_name)}</span><pre>'
+        )
 
-def exit_chunk(self) -> None:
-    self.f.write('</pre></li>')
+def exit_chunk(self, first: bool) -> None:
+    self.f.write("</pre></li>")
     self.node_path.pop()
-    super().exit_chunk()
+    super().exit_chunk(first)
 ```
 
 Now we write the methods that are called when we are ready to expand a code
 chunk name, and when we are done expanding.  There are two cases that we will
 handle.  The first case is when we are dealing with the top-level file chunks.
 In this case, we simply write an appropriate HTML header, open the `<body>`
 tag, and open a `<ul>` tag before we expand the chunks, and we close the `<ul>`
@@ -613,27 +684,30 @@
 ```{literate-code} AnnotatedTangleWriter methods
 def enter_expansion(self, chunk_name: str, is_file: bool = False) -> None:
     super().enter_expansion(chunk_name, is_file)
     if len(self.path) > self.builder.max_depth:
         self.builder.max_depth = len(self.path)
 
     if is_file:
-        self.f.write('<html><head><title>{}</title>'.format(html.escape(chunk_name)))
-        css_file = posixpath.relpath('_static/annotated.css', posixpath.dirname(self.filename))
+        self.f.write(f"<html><head><title>{chunk_name}</title>")
+        css_file = posixpath.relpath(
+            "_static/annotated.css",
+            posixpath.dirname(self.filename),
+        )
         css_file = html.escape(css_file)
-        self.f.write('<link rel="stylesheet" type="text/css" href="{}" />'.format(css_file))
-        self.f.write('</head><body><ul>')
+        self.f.write(f'<link rel="stylesheet" type="text/css" href="{css_file}"/>')
+        self.f.write("</head><body><ul>")
     else:
-        self.f.write('</pre><ul>')
+        self.f.write("</pre><ul>")
 
 def exit_expansion(self) -> None:
     if len(self.path) == 1:
-        self.f.write('</ul></body></html>')
+        self.f.write("</ul></body></html>")
     else:
-        self.f.write('</ul><pre>')
+        self.f.write("</ul><pre>")
     super().exit_expansion()
 ```
 
 ### Writing CSS
 
 To write the CSS, we first start with a base style to set up the basic
 structure.  Then, we add indentation to the `<pre>` elements.  We want the code
@@ -643,26 +717,32 @@
 2rem less for each level that it is indented.  So we create CSS rules that
 match on `ul ...(times the number of levels) pre`, and set the left margin to 2
 times (the maximum depth minus the number of levels).  And the number of such
 rules that we need to make is equal to the maximum depth.
 
 ```{literate-code} AnnotatedTangleBuilder methods
 def write_css(self) -> None:
-    os.makedirs(os.path.join(self.outdir, '_static'), exist_ok=True)
-    with open(os.path.join(self.outdir, '_static/annotated.css'), 'w') as f:
-        f.write('''
+    os.makedirs(os.path.join(self.outdir, "_static"), exist_ok=True)
+    with open(os.path.join(self.outdir, "_static/annotated.css"), "w") as f:
+        f.write(
+            """
 {{base annotations css}}
-''')
+"""
+        )
 
         for depth in range(0, self.max_depth):
-            f.write('''
+            f.write(
+                """
 ul {}pre {{
   margin-left: {}rem;
 }}
-'''.format('ul ' * depth, 2 * (self.max_depth - depth)))
+""".format(
+                    "ul " * depth, 2 * (self.max_depth - depth)
+                )
+            )
 ```
 
 ```{literate-code} base annotations css
 :lang: css
 
 html {
   background: white;
@@ -689,14 +769,20 @@
 }
 
 /* avoid doubling up borders for adjacent chunks */
 li + li {
   border-top: 0px none;
 }
 
+/* the blank line between adjacent chunks of the same name */
+li.gap {
+  border-left: 0px none;
+  margin-left: 0px
+}
+
 pre {
   margin: 0.5rem 0 0 0;
   padding: 0;
   background: LightGray;
 }
 
 pre .lineno {
@@ -711,14 +797,19 @@
   user-select: none;
   -webkit-user-select: text;
   -webkit-user-select: none;
   -moz-user-select: none;
   -ms-user-select: none;
 }
 
+li.gap > pre {
+  margin-top: 0.25rem;
+  margin-bottom: 0.25rem;
+}
+
 /* highlight the target */
 /* if the target is a line number */
 pre div:target {
   background: orange;
 }
 
 /* if the target is a chunk */
@@ -739,70 +830,83 @@
 
 ## Wrapping up
 
 Now we need to tell Sphinx about our new directive, our builders, and our
 configuration option, as well as some information about the extension.
 
 ```{literate-code} functions
+:padding: 2
+
 def setup(app: Sphinx) -> dict[str, Any]:
-    app.add_directive('literate-code', LiterateCode)
+    app.add_directive("literate-code", LiterateCode)
 
     app.add_builder(TangleBuilder)
     app.add_builder(AnnotatedTangleBuilder)
 
     app.add_config_value(
-        'literate_delimiters',
-        ('{{', # need to split this across two lines, or else when we tangle
-        '}}'), # this file, it will think it's a code chunk reference
-        'env',
+        "literate_delimiters",
+        (
+            "{{",  # need to split this across two lines, or else when we tangle
+            "}}",  # this file, it will think it's a code chunk reference
+        ),
+        "env",
         [tuple[str, str]],
     )
+    app.add_config_value(
+        "default_chunk_padding",
+        1,
+        "env",
+        int,
+    )
 
     return {
-        'version': __version__,
-        'parallel_read_safe': True,
-        'parallel_write_safe': True,
+        "version": __version__,
+        "parallel_read_safe": True,
+        "parallel_write_safe": True,
     }
 ```
 
 And we put it all together in a Python file.
 
 ```{literate-code} literate_sphinx.py
 :file:
 
 # {{copyright license}}
 
-'''A literate programming extension for Sphinx'''
+"""A literate programming extension for Sphinx"""
 
-__version__ = '0.1.2'
+__version__ = "0.1.3"
 
 from hashlib import sha256
 import html
 import io
 import os
 import posixpath
 import re
-from typing import Any, Iterator
+from typing import Any, Iterator, Optional
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from docutils.parsers.rst.roles import normalized_role_options
+from docutils.transforms import Transform
 from sphinx.application import Sphinx
 from sphinx.builders import Builder
 from sphinx.errors import ExtensionError
 from sphinx.util import logging
 from sphinx.util.console import darkgreen  # type: ignore
 from sphinx.util.docutils import SphinxDirective
 from sphinx.util.nodes import inline_all_toctrees
 
 
 logger = logging.getLogger(__name__)
 
+
 {{classes}}
 
+
 {{functions}}
 ```
 
 ## Future plans
 
 - link code chunks together
   - link to where code chunks are used
```

### Comparing `literate-sphinx-0.1.2/conf.py` & `literate-sphinx-0.1.3/conf.py`

 * *Files identical despite different names*

### Comparing `literate-sphinx-0.1.2/index.md` & `literate-sphinx-0.1.3/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,20 @@
 name of the chunk as its argument.  It takes the following options:
 
 * `lang`: the language of the chunk.  Defaults to `highlight_language`
   specified in `conf.py`
 * `file`: (takes no value) present if the chunk is a file.  If the chunk is a
   file, then the code chunk name
 * `class`: a list of class names separated by spaces to add to the HTML output
-* `name`: a target name that can be referenced by `ref` or `numrf`.  This
+* `padding`: when multiple chunks have the same name, they are written out
+  sequentially.  The `padding` indicates how many blank lines (if any) there
+  should be between this chunk and the *previous* chunk of the same name.
+  Defaults to `default_chunk_padding` specified in `conf.py`, which itself
+  defaults to 1.  If given without an argument, one blank line is used.
+* `name`: a target name that can be referenced by `ref` or `numref`.  This
   should not be confused with the code chunk name.
 
 e.g in ReST
 
 ```rst
 .. literate-code:: code chunk name
    :lang: python
```

### Comparing `literate-sphinx-0.1.2/literate_sphinx.py` & `literate-sphinx-0.1.3/literate_sphinx.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,272 +1,327 @@
 # Copyright Hubert Chathi <hubert@uhoreg.ca>
-# 
+#
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are
 # met:
-# 
+#
 # * Redistributions of source code must retain the above copyright
 #   notice, this list of conditions and the following disclaimer.
-# 
+#
 # * Redistributions in binary form must reproduce the above copyright
 #   notice, this list of conditions and the following disclaimer in the
 #   documentation and/or other materials provided with the distribution.
-# 
+#
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
 # "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
 # LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
 # A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
 # HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
 # SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 # LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 # DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 # THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-# 
+#
 # SPDX-License-Identifier: BSD-2-Clause
 
-'''A literate programming extension for Sphinx'''
+"""A literate programming extension for Sphinx"""
 
-__version__ = '0.1.2'
+__version__ = "0.1.3"
 
 from hashlib import sha256
 import html
 import io
 import os
 import posixpath
 import re
-from typing import Any, Iterator
+from typing import Any, Iterator, Optional
 
 from docutils import nodes
 from docutils.parsers.rst import directives
 from docutils.parsers.rst.roles import normalized_role_options
+from docutils.transforms import Transform
 from sphinx.application import Sphinx
 from sphinx.builders import Builder
 from sphinx.errors import ExtensionError
 from sphinx.util import logging
 from sphinx.util.console import darkgreen  # type: ignore
 from sphinx.util.docutils import SphinxDirective
 from sphinx.util.nodes import inline_all_toctrees
 
 
 logger = logging.getLogger(__name__)
 
+
 class LiterateCode(SphinxDirective):
     """Parse and mark up content of a literate code chunk.
 
     The argument is the chunk name
     """
+
     required_arguments = 1
     final_argument_whitespace = True
+
     option_spec = {
-        'class': directives.class_option,
-        'file': directives.flag,
-        'lang': directives.unchanged,
-        'name': directives.unchanged,
+        "class": directives.class_option,
+        "file": directives.flag,
+        "lang": directives.unchanged,
+        "padding": directives.unchanged,
+        "name": directives.unchanged,
     }
+
     has_content = True
 
-    def run(self) -> list[nodes.Node]:
+    def run(self) -> list[nodes.Element]:
         options = normalized_role_options(self.options)
-        language = options['lang'] if 'lang' in options else \
-            self.env.temp_data.get('highlight_language', self.config.highlight_language)
-        is_file = 'file' in options
+
+        language = (
+            options["lang"]
+            if "lang" in options
+            else self.env.temp_data.get(
+                "highlight_language", self.config.highlight_language
+            )
+        )
+
+        is_file = "file" in options
+
         chunk_name = self.arguments[0]
-        code = '\n'.join(self.content)
-    
+
+        if "padding" in options:
+            if options["padding"] == "":
+                padding = 1
+            else:
+                padding = int(options["padding"])
+        else:
+            padding = self.config.default_chunk_padding
+
+        code = "\n".join(self.content)
+
         literal_node = nodes.literal_block(code, code)
-        
-        literal_node['code-chunk-name'] = chunk_name
+
+        literal_node["code-chunk-name"] = chunk_name
         if is_file:
-            literal_node['code-chunk-is-file'] = True
-        literal_node['language'] = language
-        literal_node['classes'].append('literate-code') # allow special styling of literate blocks
-        if 'classes' in options:
-            literal_node['classes'] += options['classes']
+            literal_node["code-chunk-is-file"] = True
+        literal_node["code-chunk-padding"] = padding
+        literal_node["language"] = language
+        literal_node["classes"].append(
+            "literate-code"
+        )  # allow special styling of literate blocks
+        if "classes" in options:
+            literal_node["classes"] += options["classes"]
+
         self.set_source_info(literal_node)
-    
+
         container_node = nodes.container(
-            '', literal_block=True,
-            classes=['literal-block-wrapper', 'literate-code-wrapper']
+            "",
+            literal_block=True,
+            classes=["literal-block-wrapper", "literate-code-wrapper"],
         )
-        
+
         if is_file:
             caption_node = nodes.caption(
-                chunk_name + ':',
-                '',
+                chunk_name + ":",
+                "",
                 nodes.literal(chunk_name, chunk_name),
-                nodes.Text(':'),
+                nodes.Text(":"),
             )
         else:
-            caption_node = nodes.caption(chunk_name + ':', chunk_name + ':')
-        
+            caption_node = nodes.caption(chunk_name + ":", chunk_name + ":")
+
         self.set_source_info(caption_node)
-        
+
         container_node += caption_node
         container_node += literal_node
+
         self.add_name(container_node)
+
         return [container_node]
+
+
 class TangleBuilder(Builder):
-    name = 'tangle'
-    epilog = 'The tangled files are in %(outdir)s.'
+    name = "tangle"
+
+    epilog = "The tangled files are in %(outdir)s."
 
     def get_outdated_docs(self) -> str:
-        return 'all documents'
-    def get_target_uri(self, docname: str, typ: str = None) -> str:
-        return ''
+        return "all documents"
+
+    def get_target_uri(self, docname: str, typ: Optional[str] = None) -> str:
+        return ""
+
     def assemble_doctree(self) -> nodes.document:
         master = self.config.root_doc
         tree = self.env.get_doctree(master)
         tree = inline_all_toctrees(self, set(), master, tree, darkgreen, [master])
         return tree
+
     def write(self, *ignored: Any) -> None:
-        chunks = {} # dict of chunk name to list of chunks defined by that name
-        files = [] # the list of files
-    
+        chunks: dict[
+            str, list[nodes.Element]
+        ] = {}  # dict of chunk name to list of chunks defined by that name
+        files: list[str] = []  # the list of files
+
         doctree = self.assemble_doctree()
-    
+
         for node in doctree.findall(nodes.literal_block):
-            if 'code-chunk-name' in node:
-                name = node['code-chunk-name']
+            if "code-chunk-name" in node:
+                name = node["code-chunk-name"]
                 chunks.setdefault(name, []).append(node)
-                if 'code-chunk-is-file' in node:
+                if "code-chunk-is-file" in node:
                     files.append(name)
-    
+
         # get the delimiters from the config
         (ldelim, rdelim) = self.config.literate_delimiters
-        
+
         # get all the chunk names; initially, all chunks are unused
         unused = {name for name in chunks}
-        
+
         for filename in files:
             with self.writer(filename, unused) as writer:
                 writer.enter_expansion(filename, True)
+                first = True
                 for chunk in chunks[filename]:
-                    writer.enter_chunk(chunk)
+                    writer.enter_chunk(chunk, first)
                     for line in chunk.astext().splitlines():
-                        _write_line(writer, line, chunks, '', '', ldelim, rdelim)
-                    writer.exit_chunk()
+                        _write_line(writer, line, chunks, "", "", ldelim, rdelim)
+                    writer.exit_chunk(first)
+                    first = False
                 writer.exit_expansion()
+
         for chunk_name in unused:
             for chunk in chunks[chunk_name]:
                 logger.warning(
-                    '{0.source}:{0.line}: Code chunk "{1}" defined but not used'
-                        .format(chunk, chunk_name)
+                    '{0.source}:{0.line}: Code chunk "{1}" defined but not used'.format(
+                        chunk, chunk_name
+                    )
                 )
-    def writer(self, filename: str, unused: set[str]) -> 'TangleWriter':
+
+    def writer(self, filename: str, unused: set[str]) -> "TangleWriter":
         return TangleWriter(filename, self.outdir, unused)
+
+
 class TangleWriter:
     def __init__(
-            self,
-            filename: str,
-            outdir: str,
-            unused: set[str],
-            filename_suffix: str = ''
+        self, filename: str, outdir: str, unused: set[str], filename_suffix: str = ""
     ):
         self.unused = unused
-        self.path = []
-    
+        self.path: list[str] = []
+
         # some basic sanity checking for the file name
-        if '..' in filename or os.path.isabs(filename):
+        if ".." in filename or os.path.isabs(filename):
             raise ExtensionError(
-                "Chunk name is invalid file name: {}".format(filename),
+                f"Chunk name is invalid file name: {filename}",
                 modname=__name__,
             )
         # determine the full path, and make sure the directory exists before
         # creating the file
         fullpath = os.path.join(outdir, filename)
         dirname = os.path.dirname(fullpath)
         if dirname:
             os.makedirs(dirname, exist_ok=True)
-    
+
         self.filename = filename
-    
-        self.f = open(fullpath + filename_suffix, 'w')
+
+        self.f = open(fullpath + filename_suffix, "w")
+
     def close(self) -> None:
         self.f.close()
-    def __enter__(self) -> 'TangleWriter':
+
+    def __enter__(self) -> "TangleWriter":
         return self
-    
+
     def __exit__(self, *ignored: Any) -> None:
         self.close()
+
     def write_line(self, line: str) -> None:
-        self.f.write(line + '\n')
-    
+        self.f.write(line + "\n")
+
     def enter_expansion(self, chunk_name: str, is_file: bool = False) -> None:
         # update bookeeping variables
         self.unused.discard(chunk_name)
         if chunk_name in self.path:
             self.path.append(chunk_name)
             raise ExtensionError(
-                'Loop found in chunks: {}'.format(' -> '.join(self.path)),
-                modname = __name__,
+                "Loop found in chunks: {}".format(" -> ".join(self.path)),
+                modname=__name__,
             )
         self.path.append(chunk_name)
-    
+
     def exit_expansion(self) -> None:
         self.path.pop()
-    
-    def enter_chunk(self, chunk_node: nodes.Node) -> None:
-        pass
-    
-    def exit_chunk(self) -> None:
+
+    def enter_chunk(self, chunk_node: nodes.Element, first: bool) -> None:
+        if not first:
+            for i in range(0, chunk_node["code-chunk-padding"]):
+                self.f.write("\n")
+
+    def exit_chunk(self, first: bool) -> None:
         pass
+
+
 class AnnotatedTangleBuilder(TangleBuilder):
-    name = 'annotated-tangle'
+    name = "annotated-tangle"
 
     def writer(self, filename: str, unused: set[str]) -> TangleWriter:
         return AnnotatedTangleWriter(filename, self.outdir, unused, self)
 
     def write(self, *opts: Any) -> None:
         self.max_depth = 1
 
         super().write(*opts)
 
         self.write_css()
 
     def write_css(self) -> None:
-        os.makedirs(os.path.join(self.outdir, '_static'), exist_ok=True)
-        with open(os.path.join(self.outdir, '_static/annotated.css'), 'w') as f:
-            f.write('''
+        os.makedirs(os.path.join(self.outdir, "_static"), exist_ok=True)
+        with open(os.path.join(self.outdir, "_static/annotated.css"), "w") as f:
+            f.write(
+                """
     html {
       background: white;
       color: black;
     }
-    
+
     /* don't indent the first ul, but indent subsequent ones */
     ul {
       padding: 0;
       margin: 0;
     }
-    
+
     ul ul {
       padding-left: 1.5rem;
       margin-left: 0;
     }
-    
+
     li {
       border: 1px solid gray;
       margin-right: -1px;
       margin-left: -1px;
       padding-left: 0.5rem;
       list-style: none;
     }
-    
+
     /* avoid doubling up borders for adjacent chunks */
     li + li {
       border-top: 0px none;
     }
-    
+
+    /* the blank line between adjacent chunks of the same name */
+    li.gap {
+      border-left: 0px none;
+      margin-left: 0px
+    }
+
     pre {
       margin: 0.5rem 0 0 0;
       padding: 0;
       background: LightGray;
     }
-    
+
     pre .lineno {
       color: black;
       display: inline-block;
       width: 4em;
       text-align: right;
       border-right: 3px solid gray;
       padding-right: 0.5rem;
@@ -274,155 +329,212 @@
       background: white;
       user-select: none;
       -webkit-user-select: text;
       -webkit-user-select: none;
       -moz-user-select: none;
       -ms-user-select: none;
     }
-    
+
+    li.gap > pre {
+      margin-top: 0.25rem;
+      margin-bottom: 0.25rem;
+    }
+
     /* highlight the target */
     /* if the target is a line number */
     pre div:target {
       background: orange;
     }
-    
+
     /* if the target is a chunk */
     li:target {
       border: 3px solid orange;
       margin-right: -3px;
       margin-left: -3px;
     }
-    
+
     li:target > .chunkname{
       font-weight: bold;
     }
-    
+
     li:target pre {
       background: orange;
     }
-    ''')
-    
+    """
+            )
+
             for depth in range(0, self.max_depth):
-                f.write('''
+                f.write(
+                    """
     ul {}pre {{
       margin-left: {}rem;
     }}
-    '''.format('ul ' * depth, 2 * (self.max_depth - depth)))
+    """.format(
+                        "ul " * depth, 2 * (self.max_depth - depth)
+                    )
+                )
+
 
 class AnnotatedTangleWriter(TangleWriter):
     def __init__(
-            self,
-            filename: str,
-            outdir: str,
-            unused: set[str],
-            builder: AnnotatedTangleBuilder,
+        self,
+        filename: str,
+        outdir: str,
+        unused: set[str],
+        builder: AnnotatedTangleBuilder,
     ):
-        super().__init__(filename, outdir, unused, '.html')
+        super().__init__(filename, outdir, unused, ".html")
         self.lineno = 1
-        self.node_path = []
+        self.node_path: list[nodes.Node] = []
         self.builder = builder
+
     def write_line(self, line: str) -> None:
-        self.f.write('<div id="L{0}"><a class="lineno" href="#L{0}">{0}</a>{1}</div>'.format(self.lineno, html.escape(line)))
+        self.f.write(
+            '<div id="L{0}"><a class="lineno" href="#L{0}">{0}</a>{1}</div>'.format(
+                self.lineno, html.escape(line)
+            )
+        )
         self.lineno = self.lineno + 1
-    def enter_chunk(self, chunk_node: nodes.Node) -> None:
-        super().enter_chunk(chunk_node)
-    
+
+    def enter_chunk(self, chunk_node: nodes.Element, first: bool) -> None:
+        super().enter_chunk(chunk_node, first)
+
         self.node_path.append(chunk_node)
-        hash = sha256(':'.join(['{0.source}:{0.line}'.format(c) for c in self.node_path]).encode('utf-8')).hexdigest()
-    
-        chunk_name = chunk_node['code-chunk-name']
-        if 'code-chunk-is-file' in chunk_node:
-            self.f.write('<li id="{}"><span class="chunkname"><code>{}</code></span><pre>'.format(hash, html.escape(chunk_name)))
+        hash = sha256(
+            ":".join(["{0.source}:{0.line}".format(c) for c in self.node_path]).encode(
+                "utf-8",
+            )
+        ).hexdigest()
+
+        chunk_name = chunk_node["code-chunk-name"]
+        if not first and chunk_node["code-chunk-padding"]:
+            self.f.write('<li class="gap"><pre>')
+            for i in range(0, chunk_node["code-chunk-padding"]):
+                self.f.write(
+                    '<div id="L{0}"><a class="lineno" href="#L{0}">{0}</a></div>'.format(
+                        self.lineno,
+                    )
+                )
+                self.lineno = self.lineno + 1
+            self.f.write("</pre></li>")
+        if "code-chunk-is-file" in chunk_node:
+            self.f.write(
+                f'<li id="{hash}"><span class="chunkname"><code>{html.escape(chunk_name)}</code></span><pre>'
+            )
         else:
-            self.f.write('<li id="{}"><span class="chunkname">{}</span><pre>'.format(hash, html.escape(chunk_name)))
-    
-    def exit_chunk(self) -> None:
-        self.f.write('</pre></li>')
+            self.f.write(
+                f'<li id="{hash}"><span class="chunkname">{html.escape(chunk_name)}</span><pre>'
+            )
+
+    def exit_chunk(self, first: bool) -> None:
+        self.f.write("</pre></li>")
         self.node_path.pop()
-        super().exit_chunk()
+        super().exit_chunk(first)
+
     def enter_expansion(self, chunk_name: str, is_file: bool = False) -> None:
         super().enter_expansion(chunk_name, is_file)
         if len(self.path) > self.builder.max_depth:
             self.builder.max_depth = len(self.path)
-    
+
         if is_file:
-            self.f.write('<html><head><title>{}</title>'.format(html.escape(chunk_name)))
-            css_file = posixpath.relpath('_static/annotated.css', posixpath.dirname(self.filename))
+            self.f.write(f"<html><head><title>{chunk_name}</title>")
+            css_file = posixpath.relpath(
+                "_static/annotated.css",
+                posixpath.dirname(self.filename),
+            )
             css_file = html.escape(css_file)
-            self.f.write('<link rel="stylesheet" type="text/css" href="{}" />'.format(css_file))
-            self.f.write('</head><body><ul>')
+            self.f.write(f'<link rel="stylesheet" type="text/css" href="{css_file}"/>')
+            self.f.write("</head><body><ul>")
         else:
-            self.f.write('</pre><ul>')
-    
+            self.f.write("</pre><ul>")
+
     def exit_expansion(self) -> None:
         if len(self.path) == 1:
-            self.f.write('</ul></body></html>')
+            self.f.write("</ul></body></html>")
         else:
-            self.f.write('</ul><pre>')
+            self.f.write("</ul><pre>")
         super().exit_expansion()
 
+
 def _write_line(
-        writer: TangleWriter,
-        line: str,
-        chunks: dict[str, Any],
-        prefix: str,
-        suffix: str,
-        ldelim: str,
-        rdelim: str,
+    writer: TangleWriter,
+    line: str,
+    chunks: dict[str, Any],
+    prefix: str,
+    suffix: str,
+    ldelim: str,
+    rdelim: str,
 ) -> None:
     # check if the line contains the left and right delimiter
     s1 = line.split(ldelim, 1)
     if len(s1) == 2:
         s2 = s1[1].rsplit(rdelim, 1)
         if len(s2) == 2:
             # delimiters found, so get the chunk name
             chunk_name = s2[0].strip()
 
             # write the chunks associated with the name
             try:
                 ref_chunks = chunks[chunk_name]
             except KeyError:
                 raise ExtensionError(
-                    'Unknown chunk name: {}'.format(chunk_name),
-                    modname = __name__,
+                    f"Unknown chunk name: {chunk_name}",
+                    modname=__name__,
                 )
             writer.enter_expansion(chunk_name)
+            first = True
             for ins_chunk in ref_chunks:
-                writer.enter_chunk(ins_chunk)
+                writer.enter_chunk(ins_chunk, first)
                 for ins_line in ins_chunk.astext().splitlines():
                     # recursively call this function with each line of the
                     # referenced code chunks
                     _write_line(
                         writer,
                         ins_line,
                         chunks,
                         prefix + s1[0],
                         s2[1] + suffix,
                         ldelim,
                         rdelim,
                     )
-                writer.exit_chunk()
+                writer.exit_chunk(first)
+                first = False
             writer.exit_expansion()
 
             return
 
     # delimiters not found, so just write the line
-    writer.write_line(prefix + line + suffix)
+    if not line and not suffix:
+        # if line and suffix are both blank, strip off trailing whitespace
+        # from the prefix
+        writer.write_line(prefix.rstrip())
+    else:
+        writer.write_line(prefix + line + suffix)
+
+
 def setup(app: Sphinx) -> dict[str, Any]:
-    app.add_directive('literate-code', LiterateCode)
+    app.add_directive("literate-code", LiterateCode)
 
     app.add_builder(TangleBuilder)
     app.add_builder(AnnotatedTangleBuilder)
 
     app.add_config_value(
-        'literate_delimiters',
-        ('{{', # need to split this across two lines, or else when we tangle
-        '}}'), # this file, it will think it's a code chunk reference
-        'env',
+        "literate_delimiters",
+        (
+            "{{",  # need to split this across two lines, or else when we tangle
+            "}}",  # this file, it will think it's a code chunk reference
+        ),
+        "env",
         [tuple[str, str]],
     )
+    app.add_config_value(
+        "default_chunk_padding",
+        1,
+        "env",
+        int,
+    )
 
     return {
-        'version': __version__,
-        'parallel_read_safe': True,
-        'parallel_write_safe': True,
+        "version": __version__,
+        "parallel_read_safe": True,
+        "parallel_write_safe": True,
     }
```

### Comparing `literate-sphinx-0.1.2/make.bat` & `literate-sphinx-0.1.3/make.bat`

 * *Files identical despite different names*

### Comparing `literate-sphinx-0.1.2/pyproject.toml` & `literate-sphinx-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -27,7 +27,13 @@
 Documentation = "https://uhoreg.gitlab.io/literate-sphinx/"
 Source = "https://gitlab.com/uhoreg/literate-sphinx"
 
 [project.optional-dependencies]
 build = [
     "myst-parser",
 ]
+
+lint = [
+    "black",
+    "types-docutils",
+    "mypy",
+]
```

### Comparing `literate-sphinx-0.1.2/requirements.txt` & `literate-sphinx-0.1.3/requirements.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 alabaster==0.7.13
 Babel==2.11.0
+black==23.7.0
 certifi==2022.12.7
 charset-normalizer==3.0.1
+click==8.1.6
 docutils==0.19
 flit==3.8.0
-flit-core==3.8.0
+flit_core==3.8.0
 idna==3.4
 imagesize==1.4.1
 importlib-metadata==6.0.0
 Jinja2==3.1.2
 markdown-it-py==2.1.0
 MarkupSafe==2.1.1
 mdit-py-plugins==0.3.3
 mdurl==0.1.2
+mypy==1.4.1
+mypy-extensions==1.0.0
 myst-parser==0.18.1
 packaging==23.0
+pathspec==0.11.1
+platformdirs==3.9.1
 Pygments==2.14.0
 pytz==2022.7.1
-PyYAML==6.0
+PyYAML==6.0.1
 requests==2.28.2
 snowballstemmer==2.2.0
-sphinx==5.3.0
-sphinxcontrib-applehelp==1.0.3
+Sphinx==5.3.0
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.0
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-tomli-w==1.0.0
-typing-extensions==4.4.0
+sphinxcontrib.applehelp==1.0.3
+tomli_w==1.0.0
+types-docutils==0.20.0.1
+typing_extensions==4.4.0
 urllib3==1.26.14
 zipp==3.11.0
```

### Comparing `literate-sphinx-0.1.2/PKG-INFO` & `literate-sphinx-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: literate-sphinx
-Version: 0.1.2
+Version: 0.1.3
 Summary: A literate programming extension for Sphinx
 Keywords: sphinx,literate programming
 Author-email: Hubert Chathi <hubert@uhoreg.ca>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Requires-Dist: sphinx
 Requires-Dist: myst-parser ; extra == "build"
+Requires-Dist: black ; extra == "lint"
+Requires-Dist: types-docutils ; extra == "lint"
+Requires-Dist: mypy ; extra == "lint"
 Project-URL: Documentation, https://uhoreg.gitlab.io/literate-sphinx/
 Project-URL: Home, https://gitlab.com/uhoreg/literate-sphinx/
 Project-URL: Source, https://gitlab.com/uhoreg/literate-sphinx
 Provides-Extra: build
+Provides-Extra: lint
 
 # Literate Sphinx
 
 Literate Sphinx is a [literate
 programming](https://en.wikipedia.org/wiki/Literate_programming) extension for
 [Sphinx](https://www.sphinx-doc.org/).  Literate programming is a method for
 writing code interleaved with text.  With literate programming, code is
@@ -43,15 +47,20 @@
 name of the chunk as its argument.  It takes the following options:
 
 * `lang`: the language of the chunk.  Defaults to `highlight_language`
   specified in `conf.py`
 * `file`: (takes no value) present if the chunk is a file.  If the chunk is a
   file, then the code chunk name
 * `class`: a list of class names separated by spaces to add to the HTML output
-* `name`: a target name that can be referenced by `ref` or `numrf`.  This
+* `padding`: when multiple chunks have the same name, they are written out
+  sequentially.  The `padding` indicates how many blank lines (if any) there
+  should be between this chunk and the *previous* chunk of the same name.
+  Defaults to `default_chunk_padding` specified in `conf.py`, which itself
+  defaults to 1.  If given without an argument, one blank line is used.
+* `name`: a target name that can be referenced by `ref` or `numref`.  This
   should not be confused with the code chunk name.
 
 e.g in ReST
 
 ```rst
 .. literate-code:: code chunk name
    :lang: python
```

