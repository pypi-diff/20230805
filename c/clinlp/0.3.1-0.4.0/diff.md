# Comparing `tmp/clinlp-0.3.1.tar.gz` & `tmp/clinlp-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clinlp-0.3.1.tar", max compression
+gzip compressed data, was "clinlp-0.4.0.tar", max compression
```

## Comparing `clinlp-0.3.1.tar` & `clinlp-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-06-30 11:47:19.186990 clinlp-0.3.1/LICENSE
--rw-r--r--   0        0        0     9454 2023-06-30 11:47:19.186990 clinlp-0.3.1/README.md
--rw-r--r--   0        0        0      162 2023-06-30 11:47:19.186990 clinlp-0.3.1/clinlp/__init__.py
--rw-r--r--   0        0        0     8597 2023-06-30 11:47:19.186990 clinlp-0.3.1/clinlp/language.py
--rw-r--r--   0        0        0     1603 2023-06-30 11:47:19.186990 clinlp-0.3.1/clinlp/normalizer.py
--rw-r--r--   0        0        0      197 2023-06-30 11:47:19.186990 clinlp-0.3.1/clinlp/qualifier/__init__.py
--rw-r--r--   0        0        0    11580 2023-06-30 11:47:19.186990 clinlp-0.3.1/clinlp/qualifier/context_algorithm.py
--rw-r--r--   0        0        0      975 2023-06-30 11:47:19.186990 clinlp-0.3.1/clinlp/qualifier/qualifier.py
--rw-r--r--   0        0        0     4374 2023-06-30 11:47:19.186990 clinlp-0.3.1/clinlp/qualifier/transformer.py
--rw-r--r--   0        0        0        0 2023-06-30 11:47:19.186990 clinlp-0.3.1/clinlp/resources/__init__.py
--rw-r--r--   0        0        0    24490 2023-06-30 11:47:19.186990 clinlp-0.3.1/clinlp/resources/psynlp_context_rules.json
--rw-r--r--   0        0        0     2272 2023-06-30 11:47:19.186990 clinlp-0.3.1/clinlp/sentencizer.py
--rw-r--r--   0        0        0     1815 2023-06-30 11:47:19.186990 clinlp-0.3.1/clinlp/util.py
--rw-r--r--   0        0        0      678 2023-06-30 11:47:19.190990 clinlp-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    10112 1970-01-01 00:00:00.000000 clinlp-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-05 13:21:56.612014 clinlp-0.4.0/LICENSE
+-rw-r--r--   0        0        0     9473 2023-08-05 13:21:56.612014 clinlp-0.4.0/README.md
+-rw-r--r--   0        0        0      269 2023-08-05 13:21:56.612014 clinlp-0.4.0/clinlp/__init__.py
+-rw-r--r--   0        0        0       48 2023-08-05 13:21:56.612014 clinlp-0.4.0/clinlp/exceptions.py
+-rw-r--r--   0        0        0     8662 2023-08-05 13:21:56.612014 clinlp-0.4.0/clinlp/language.py
+-rw-r--r--   0        0        0     1603 2023-08-05 13:21:56.612014 clinlp-0.4.0/clinlp/normalizer.py
+-rw-r--r--   0        0        0      300 2023-08-05 13:21:56.612014 clinlp-0.4.0/clinlp/qualifier/__init__.py
+-rw-r--r--   0        0        0    11572 2023-08-05 13:21:56.612014 clinlp-0.4.0/clinlp/qualifier/context_algorithm.py
+-rw-r--r--   0        0        0     2605 2023-08-05 13:21:56.612014 clinlp-0.4.0/clinlp/qualifier/qualifier.py
+-rw-r--r--   0        0        0     4746 2023-08-05 13:21:56.612014 clinlp-0.4.0/clinlp/qualifier/transformer.py
+-rw-r--r--   0        0        0        0 2023-08-05 13:21:56.612014 clinlp-0.4.0/clinlp/resources/__init__.py
+-rw-r--r--   0        0        0    26423 2023-08-05 13:21:56.612014 clinlp-0.4.0/clinlp/resources/context_rules.json
+-rw-r--r--   0        0        0     2272 2023-08-05 13:21:56.612014 clinlp-0.4.0/clinlp/sentencizer.py
+-rw-r--r--   0        0        0     1815 2023-08-05 13:21:56.612014 clinlp-0.4.0/clinlp/util.py
+-rw-r--r--   0        0        0      678 2023-08-05 13:21:56.616014 clinlp-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    10131 1970-01-01 00:00:00.000000 clinlp-0.4.0/PKG-INFO
```

### Comparing `clinlp-0.3.1/LICENSE` & `clinlp-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clinlp-0.3.1/README.md` & `clinlp-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 
 text = (
     "Patiente bij mij gezien op spreekuur, omdat zij vorige maand verlies van "
     "reuk na covid infectie aangaf. Zij had geen last meer van kortademigheid, "
     "wel was er nog sprake van hoesten, geen afname vermoeidheid."
 )
 
-
 doc = nlp(text)
 ```
 
 Find information in the doc object:
 
 ```python
 from spacy import displacy
@@ -71,15 +70,15 @@
 
 ![example_doc_render.png](media/example_doc_render.png)
 
 With relevant qualifiers:
 
 ```python
 for ent in doc.ents:
-  print(ent, ent.start, ent.end, ent._.qualifiers)
+  print(ent.start, ent.end, ent, ent._.qualifiers_str)
 
 ```
 
 * `11` `14` `verlies van reuk` `{'Temporality.HISTORICAL'}`
 * `25` `26` `kortademigheid` `{'Negation.NEGATED'}`
 * `33` `34` `hoesten` `{}`
 * `37` `38` `vermoeidheid` `{}`
@@ -115,15 +114,15 @@
 - Regarding [DEDUCE](https://github.com/vmenger/deduce) tags as a single token (e.g. `[DATUM-1]`). 
   - Deidentification is not builtin `clinlp` and should be done as a preprocessing step.
 
 ### Normalizer
 
 The normalizer sets the `token.norm` attribute, which can be used by further components (entity recognition, qualification) for matching. It currently has two options (enabled by default):
 - Lowercasing
-- Removing diacritings, where possible. For instance, it will map `ë` `->` `e`, but keeps most other non-ascii characters intact (e.g. `µ`, `²`).
+- Removing diacritics, where possible. For instance, it will map `ë` `->` `e`, but keeps most other non-ascii characters intact (e.g. `µ`, `²`).
 
 Note that this component only has effect when explicitly configuring successor components to match on the `token.norm` attribute. 
 
 ### Sentence splitter
 
 The sentence splitter can be added as follows:
 
@@ -131,17 +130,17 @@
 nlp.add_pipe('clinlp_sentencizer')
 ```
 
 It is designed to detect sentence boundaries in clinical text, whenever a character that demarks a sentence ending is matched (e.g. newline, period, question mark). It also correctly detects items in an enumerations (e.g. starting with `-` or `*`). 
 
 ### Entity matcher
 
-Currently, the spaCy builtin `PhraseMatcher` and `Matcher` can be used for finding (named) entities in text. The first one accepts literal phrases only, that are matched in the tokenized text, while the second one also accepts [spaCy patterns](https://spacy.io/usage/rule-based-matching#adding-patterns). These are not tailored for the clinical domain, but nevertheless useful when a somewhat coherent list of relevant patterns can be generated/obtained.
+Currently, the spaCy builtin `EntityRuler` can be used for finding (named) entities in text. It accepts both literal phrases (single terms or multi-word expressions) and [spaCy patterns](https://spacy.io/usage/rule-based-matching#adding-patterns), which give more control over the specific sequence of tokens to match. The spaCy `EntityRuler` is not necessarily tailored for the clinical domain, but nevertheless useful when a somewhat coherent list of relevant patterns can be generated/obtained. A better or more specific NER module will hopefully be added in the future. 
 
-For instance, a matcher that helps recognize COVID19 symptoms:
+For instance, a matcher that helps recognize COVID-19 symptoms:
 
 ```python
 ruler = nlp.add_pipe('entity_ruler', config={'phrase_matcher_attr': "NORM"})
 
 terms = {
     'covid_19_symptomen': [
         'verkouden', 'neusverkouden', 'loopneus', 'niezen', 
@@ -151,27 +150,26 @@
 }
 
 for term_description, terms in terms.items():
     ruler.add_patterns([{'label': term_description, 'pattern': term} for term in terms])
 ```
 
 For more info, it's useful to check out these spaCy documentation pages:
+* [[spaCy API] EntityRuler](https://spacy.io/api/entityruler)
 * [Rule based matching](https://spacy.io/usage/rule-based-matching)
-* [[spaCy API] Matcher](https://spacy.io/api/matcher)
-* [[spaCy API] PhraseMatcher](https://spacy.io/api/phrasematcher)
 
-Note that the `DependencyMatcher` cannot be used, and neither are part of speech tags available, as no good models for determining this information for clinical text exist (yet).  
+Note that Part of Speech tags and dependency trees and cannot be used in `clinlp`, as no good models for determining this information for clinical text exist (yet).  
 
 ### Qualifier detection
 
-After finding entities, it's often useful to qualify these entities, e.g.: are they negated or affirmed, historical or current? `clinlp` currently implements the rule-based [Context algorithm](https://doi.org/10.1016%2Fj.jbi.2009.05.002), and a [transformer-based negation detector](https://doi.org/10.48550/arxiv.2209.00470). 
+After finding entities, it's often useful to qualify these entities, e.g.: are they negated or affirmed, historical or current? `clinlp` currently implements two options: the rule-based Context Algorithm, and a transformer-based negation detector. 
 
 #### Context Algorithm
 
-The rule-based Context Algorithm is fairly accurate, and quite transparent and fast. A set of rules, that checks for negation, temporality, plausibility and experiencer, is loaded by default:
+The rule-based [Context Algorithm](https://doi.org/10.1016%2Fj.jbi.2009.05.002) is fairly accurate, and quite transparent and fast. A set of rules, that checks for negation, temporality, plausibility and experiencer, is loaded by default:
 
 ```python
 nlp.add_pipe('clinlp_context_algorithm', config={'phrase_matcher_attr': 'NORM'})
 ```
 
 A custom set of rules, including different types of qualifiers, can easily be defined. See [`clinlp/resources/psynlp_context_rules.json`](clinlp/resources/psynlp_context_rules.json) for an example, and load it as follows:
```

### Comparing `clinlp-0.3.1/clinlp/language.py` & `clinlp-0.4.0/clinlp/language.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 import spacy.lang.nl.tokenizer_exceptions
 import spacy.lang.punctuation
 import spacy.lang.tokenizer_exceptions
 from spacy.language import BaseDefaults, Language
 from spacy.symbols import ORTH
 from spacy.util import update_exc
 
+from clinlp.exceptions import VersionMismatchWarning
+
 CLINLP_ABBREVIATIONS = [
     "dhr.",
     "dr.",
     "dh.",
     "drs.",
     "ds.",
     "gg.",
@@ -400,13 +402,13 @@
 
         if "clinlp_version" in meta:
             if meta["clinlp_version"] != clinlp_version:
                 warnings.warn(
                     f"This spaCy model was built with clinlp version {meta['clinlp_version']}, "
                     f"but you currently have version {clinlp_version} installed, "
                     f"potentially leading to unexpected results.",
-                    UserWarning,
+                    VersionMismatchWarning,
                 )
         else:
             meta["clinlp_version"] = clinlp_version
 
         super().__init__(*args, meta=meta, **kwargs)
```

### Comparing `clinlp-0.3.1/clinlp/normalizer.py` & `clinlp-0.4.0/clinlp/normalizer.py`

 * *Files identical despite different names*

### Comparing `clinlp-0.3.1/clinlp/qualifier/context_algorithm.py` & `clinlp-0.4.0/clinlp/qualifier/context_algorithm.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,20 @@
 from typing import Iterator, Optional, Union
 
 import intervaltree as ivt
 from spacy.language import Language
 from spacy.matcher import Matcher, PhraseMatcher
 from spacy.tokens import Doc, Span
 
-from clinlp.qualifier.qualifier import QUALIFIERS_ATTR, Qualifier, QualifierDetector
+from clinlp.qualifier.qualifier import (
+    ATTR_QUALIFIERS,
+    Qualifier,
+    QualifierDetector,
+    QualifierFactory,
+)
 from clinlp.util import clinlp_autocomponent
 
 
 class ContextRuleDirection(Enum):
     """
     Direction of a Context rule, as in the original Context Algorithm.
     """
@@ -74,22 +79,22 @@
         elif self.rule.direction == ContextRuleDirection.FOLLOWING:
             self.scope = (max(self.start - max_scope, sentence.start), self.end)
 
 
 _defaults_context_algorithm = {
     "phrase_matcher_attr": "TEXT",
     "load_rules": True,
-    "rules": str(importlib.resources.path("clinlp.resources", "psynlp_context_rules.json")),
+    "rules": str(importlib.resources.path("clinlp.resources", "context_rules.json")),
 }
 
 
 @Language.factory(
     name="clinlp_context_algorithm",
     requires=["doc.sents", "doc.ents"],
-    assigns=[f"span._.{QUALIFIERS_ATTR}"],
+    assigns=[f"span._.{ATTR_QUALIFIERS}"],
     default_config=_defaults_context_algorithm,
 )
 @clinlp_autocomponent
 class ContextAlgorithm(QualifierDetector):
     """
     Implements the Context algorithm (https://doi.org/10.1016%2Fj.jbi.2009.05.002) as a spaCy pipeline component.
 
@@ -144,36 +149,37 @@
         """
         Add multiple rules.
         """
         for rule in rules:
             self.add_rule(rule)
 
     @staticmethod
-    def _parse_qualifier(qualifier: str, qualifier_classes: dict[str, Qualifier]) -> Qualifier:
+    def _parse_qualifier(qualifier: str, factories: dict[str, QualifierFactory]) -> Qualifier:
         """
         Parse a Qualifier from string.
 
         Args:
             qualifier: The qualifier (e.g. Negation.NEGATED).
-            qualifier_classes: A mapping of string to qualifier class.
+            factories: A mapping of string to qualifier class.
 
         Returns: A qualifier, as specified.
         """
 
         match_regexp = r"\w+\.\w+"
 
         if not re.match(match_regexp, qualifier):
             raise ValueError(
                 f"Cannot parse qualifier {qualifier}, please adhere to format "
                 f"{match_regexp} (e.g. NegationQualifier.NEGATED)"
             )
 
         qualifier_class, qualifier = qualifier.split(".")
+        qualifier_factory = factories[qualifier_class]
 
-        return qualifier_classes[qualifier_class][qualifier]
+        return qualifier_factory.get_qualifier(value=qualifier)
 
     @staticmethod
     def _parse_direction(direction: str) -> ContextRuleDirection:
         """
         Parse a Context direction.
 
         Args:
@@ -184,23 +190,23 @@
         return ContextRuleDirection[direction.upper()]
 
     def _parse_rules(self, rules: Union[str | dict]) -> list[ContextRule]:
         if isinstance(rules, str):
             with open(rules, "rb") as file:
                 rules = json.load(file)
 
-        qualifiers = {
-            qualifier["qualifier"]: Qualifier(qualifier["qualifier"], qualifier["values"])
+        factories = {
+            qualifier["name"]: QualifierFactory(qualifier["name"], qualifier["values"])
             for qualifier in rules["qualifiers"]
         }
 
         qualifier_rules = []
 
         for rule in rules["rules"]:
-            qualifier = self._parse_qualifier(rule["qualifier"], qualifiers)
+            qualifier = self._parse_qualifier(rule["qualifier"], factories)
             direction = self._parse_direction(rule["direction"])
             max_scope = rule.get("max_scope", None)
 
             qualifier_rules += [ContextRule(pattern, qualifier, direction, max_scope) for pattern in rule["patterns"]]
 
         return qualifier_rules
 
@@ -221,17 +227,15 @@
     def _group_matched_patterns(matched_patterns: list[_MatchedContextPattern]) -> defaultdict:
         """
         Group matched patterns by qualifier and direction.
         """
         groups = defaultdict(lambda: defaultdict(list))
 
         for matched_rule in matched_patterns:
-            groups[matched_rule.rule.qualifier][matched_rule.rule.direction.name].append(
-                matched_rule
-            )  # TODO: don't use name?
+            groups[matched_rule.rule.qualifier][matched_rule.rule.direction].append(matched_rule)
 
         return groups
 
     @staticmethod
     def _limit_scopes_from_terminations(
         scopes: ivt.IntervalTree, terminations: list[_MatchedContextPattern]
     ) -> ivt.IntervalTree:
@@ -256,19 +260,19 @@
 
     def _compute_match_scopes(self, matched_patterns: list[_MatchedContextPattern]) -> ivt.IntervalTree:
         """
         Compute the scope for each matched pattern, return them as an IntervalTree.
         """
         match_scopes = ivt.IntervalTree()
 
-        for _, qualifier_matches in self._group_matched_patterns(matched_patterns).items():
-            preceding = qualifier_matches[ContextRuleDirection.PRECEDING.name]
-            following = qualifier_matches[ContextRuleDirection.FOLLOWING.name]
-            pseudo = qualifier_matches[ContextRuleDirection.PSEUDO.name]
-            termination_ = qualifier_matches[ContextRuleDirection.TERMINATION.name]
+        for qualifier_matches in self._group_matched_patterns(matched_patterns).values():
+            preceding = qualifier_matches[ContextRuleDirection.PRECEDING]
+            following = qualifier_matches[ContextRuleDirection.FOLLOWING]
+            pseudo = qualifier_matches[ContextRuleDirection.PSEUDO]
+            termination = qualifier_matches[ContextRuleDirection.TERMINATION]
 
             qualifier_matches = ivt.IntervalTree()
 
             # Following, preceding
             for match in preceding + following:
                 qualifier_matches[match.start : match.end] = match
 
@@ -277,15 +281,15 @@
                 qualifier_matches.remove_overlap(match.start, match.end)
 
             # Termination
             qualifier_scopes = ivt.IntervalTree(
                 ivt.Interval(i.data.scope[0], i.data.scope[1], i.data) for i in qualifier_matches
             )
 
-            match_scopes |= self._limit_scopes_from_terminations(qualifier_scopes, termination_)
+            match_scopes |= self._limit_scopes_from_terminations(qualifier_scopes, termination)
 
         return match_scopes
 
     def detect_qualifiers(self, doc: Doc):
         """
         Apply the Context Algorithm to a doc.
         """
```

### Comparing `clinlp-0.3.1/clinlp/qualifier/transformer.py` & `clinlp-0.4.0/clinlp/qualifier/transformer.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,53 +2,60 @@
 from typing import Callable, Optional, Tuple
 
 import torch
 from spacy import Language
 from spacy.tokens import Doc, Span
 from transformers import AutoTokenizer, RobertaForTokenClassification
 
-from clinlp.qualifier.qualifier import QUALIFIERS_ATTR, Qualifier, QualifierDetector
+from clinlp.qualifier.qualifier import (
+    ATTR_QUALIFIERS,
+    QualifierDetector,
+    QualifierFactory,
+)
 from clinlp.util import clinlp_autocomponent
 
 TRANSFORMER_REPO = "UMCU/MedRoBERTa.nl_NegationDetection"
 
 _defaults_negation_transformer = {
     "token_window": 32,
     "strip_entities": True,
     "placeholder": None,
     "probas_aggregator": statistics.mean,
     "negation_threshold": 0.5,
+    "affirmed_threshold": 0.5,
 }
 
 
 @Language.factory(
     name="clinlp_negation_transformer",
     requires=["doc.ents"],
-    assigns=[f"span._.{QUALIFIERS_ATTR}"],
+    assigns=[f"span._.{ATTR_QUALIFIERS}"],
     default_config=_defaults_negation_transformer,
 )
 @clinlp_autocomponent
 class NegationTransformer(QualifierDetector):
     def __init__(
         self,
         nlp: Language,
         token_window: int = _defaults_negation_transformer["token_window"],
         strip_entities: bool = _defaults_negation_transformer["strip_entities"],
         placeholder: Optional[str] = _defaults_negation_transformer["placeholder"],
         probas_aggregator: Callable = _defaults_negation_transformer["probas_aggregator"],
         negation_threshold: float = _defaults_negation_transformer["negation_threshold"],
+        affirmed_threshold: float = _defaults_negation_transformer["affirmed_threshold"],
     ):
         self.nlp = nlp
         self.token_window = token_window
         self.strip_entities = strip_entities
         self.placeholder = placeholder
         self.probas_aggregator = probas_aggregator
         self.negation_threshold = negation_threshold
+        self.affirmed_threshold = affirmed_threshold
 
-        self.negation_qualifier = Qualifier("Negation", ["AFFIRMED", "NEGATED"])
+        self.negation_factory = QualifierFactory("Negation", ["AFFIRMED", "UNKNOWN", "NEGATED"])
 
         self.tokenizer = AutoTokenizer.from_pretrained(TRANSFORMER_REPO)
         self.model = RobertaForTokenClassification.from_pretrained(TRANSFORMER_REPO)
 
     @staticmethod
     def _get_ent_window(ent: Span, token_window: int) -> Tuple[str, int, int]:
         start_token_i = max(0, ent.start - token_window)
@@ -99,14 +106,15 @@
                 text, ent_start_char, ent_end_char = self._trim_ent_boundaries(text, ent_start_char, ent_end_char)
 
             if self.placeholder is not None:
                 text, ent_start_char, ent_end_char = self._fill_ent_placeholder(
                     text, ent_start_char, ent_end_char, placeholder=self.placeholder
                 )
 
-            if (
-                self._get_negation_prob(text, ent_start_char, ent_end_char, probas_aggregator=self.probas_aggregator)
-                > self.negation_threshold
-            ):
-                self.add_qualifier_to_ent(ent, self.negation_qualifier.NEGATED)
+            prob = self._get_negation_prob(text, ent_start_char, ent_end_char, probas_aggregator=self.probas_aggregator)
+
+            if prob > self.negation_threshold:
+                self.add_qualifier_to_ent(ent, self.negation_factory.get_qualifier("NEGATED", prob=prob))
+            elif prob > self.affirmed_threshold:
+                self.add_qualifier_to_ent(ent, self.negation_factory.get_qualifier("UNKNOWN", prob=prob))
 
         return doc
```

### Comparing `clinlp-0.3.1/clinlp/resources/psynlp_context_rules.json` & `clinlp-0.4.0/clinlp/resources/context_rules.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7882924906781733%*

 * *Differences: {"'description'": "'A set of context rules intially based on the psynlp package, somewhat tailored "*

 * *                  "on a per use case basis.'",*

 * * "'qualifiers'": "{0: {'name': 'Experiencer', delete: ['qualifier']}, 1: {'name': 'Negation', "*

 * *                 "delete: ['qualifier']}, 2: {'name': 'Plausibility', delete: ['qualifier']}, 3: "*

 * *                 "{'name': 'Temporality', delete: ['qualifier']}}",*

 * * "'rules'": "{0: {'patterns': {insert: [(0, 'familieanamnese'), (1, 'familie-anamnese'), (2, "*

 * *       […]*

```diff
@@ -1,44 +1,47 @@
 {
-    "description": "A set of context rules based on the psynlp package, a rule-based approach somewhat tailored to information extraction from clinical text.",
+    "description": "A set of context rules intially based on the psynlp package, somewhat tailored on a per use case basis.",
     "name": "default_qualifiers",
     "qualifiers": [
         {
-            "qualifier": "Experiencer",
+            "name": "Experiencer",
             "values": [
                 "PATIENT",
                 "OTHER"
             ]
         },
         {
-            "qualifier": "Negation",
+            "name": "Negation",
             "values": [
                 "AFFIRMED",
                 "NEGATED"
             ]
         },
         {
-            "qualifier": "Plausibility",
+            "name": "Plausibility",
             "values": [
                 "PLAUSIBLE",
                 "HYPOTHETICAL"
             ]
         },
         {
-            "qualifier": "Temporality",
+            "name": "Temporality",
             "values": [
                 "CURRENT",
                 "HISTORICAL"
             ]
         }
     ],
     "rules": [
         {
             "direction": "preceding",
             "patterns": [
+                "familieanamnese",
+                "familie-anamnese",
+                "familie anamnese",
                 "familiair",
                 "familiaire",
                 "familieleden",
                 "familiegeschiedenis",
                 "moederszijde",
                 "vaderszijde",
                 [
@@ -526,27 +529,25 @@
                 "geen",
                 "is geen",
                 "is niet",
                 "konden geen",
                 "konden niet",
                 "kunnen geen",
                 "kunnen niet",
-                "nam af",
                 "negatief voor",
                 "niet waarschijnlijk",
                 "niet",
                 "nooit last gehad van",
                 "nooit",
                 "ontkend",
                 "ontkennend",
                 "ontkent",
                 "ontwikkelde geen",
                 "ontwikkelde nooit",
                 "ontwikkelt geen",
-                "onwaarschijnlijk",
                 "patient is niet",
                 "patient was niet",
                 "sluit uit",
                 "subklinisch",
                 "subklinische",
                 "toonde geen",
                 "toonde geen",
@@ -567,30 +568,27 @@
             "qualifier": "Negation.NEGATED"
         },
         {
             "direction": "following",
             "max_scope": 5,
             "patterns": [
                 "afwezig",
+                "gestaakt",
                 "is uitgesloten",
                 "is verdwenen",
                 "is weg",
                 "kan worden uitgesloten",
-                "laag ingeschat",
-                "nam af",
                 "niet aan de orde",
                 "niet aanwezig",
-                "niet besproken",
                 "niet gezien",
                 "niet meer",
-                "niet waarschijnlijk",
-                "onwaarschijnlijk",
                 "opgelost",
-                "preventieplan",
                 "speelt niet",
+                "in complete remissie",
+                "in totale remissie",
                 "waren niet",
                 "was niet",
                 "werd uitgesloten",
                 "werden ontkend",
                 "werden uitgesloten",
                 "worden ontkend",
                 "zijn afwezig",
@@ -605,36 +603,30 @@
             "direction": "pseudo",
             "patterns": [
                 "geen afname",
                 "geen oorzaak van",
                 "geen toename",
                 "geen verandering",
                 "geen verbetering",
-                "geen verdere",
+                "geen verklaring",
                 "geen zekere verandering",
                 "gram negatief",
-                "herkent zich niet",
-                "is misschien niet",
-                "is mogelijk niet",
                 "kan niet",
-                "misschien niet",
-                "mogelijk niet",
                 "niet alleen",
                 "niet besproken",
                 "niet duidelijk",
                 "niet gevraagd",
+                "niet geindiceerd",
                 "niet mogelijk om ",
-                "niet noodzakelijkerwijs",
-                "niet perse",
                 "niet uit te sluiten",
                 "niet uitgesloten",
                 "niet uitgevraagd",
-                "niet uitgevraagd",
                 "niet zeker of",
                 "wel of niet",
+                "zonder effect op",
                 "zonder moeite",
                 "zonder moelijkheid",
                 "zonder verdere",
                 "niet goed"
             ],
             "qualifier": "Negation.NEGATED"
         },
@@ -751,73 +743,113 @@
                 "kan",
                 "kans op",
                 "mgl",
                 "mogelijk gerelateerd aan",
                 "mogelijk",
                 "mogelijke",
                 "neiging tot",
+                "niet besproken",
                 "niet duidelijk",
                 "observeren van",
                 "onduidelijk",
+                "onwaarschijnlijk",
                 "rekening houden met",
                 "risico op",
+                "screen",
+                "screening",
+                "te verwachten",
                 "twijfel",
                 "uitsluiten",
                 "verdenking",
                 "vermoedde",
                 "vermoedden",
                 "vermoeden van",
                 "vermoeden",
                 "vermoedt",
+                "verwachte",
                 "voorlopige diagnose",
+                "waarschijnlijk",
                 "wanneer",
                 "wel of niet",
                 "wordt gedacht aan",
                 "zorgen voor",
                 "zou",
+                "werkdiagnose",
                 "dan"
             ],
             "qualifier": "Plausibility.HYPOTHETICAL"
         },
         {
             "direction": "following",
             "patterns": [
                 "?",
                 "ambivalent",
+                "kan niet worden uitgesloten",
                 "kan worden",
                 "kan zijn",
+                "kon niet worden uitgesloten",
                 "niet besproken",
                 "niet duidelijk",
                 "niet uitgevraagd",
+                "niet uit te sluiten",
+                "niet waarschijnlijk",
+                "screen",
+                "screening",
                 "onduidelijk",
+                "onwaarschijnijk",
                 "vermoedde",
                 "vermoedden",
+                "waarschijnlijk",
                 "zou worden",
                 "zou zijn"
             ],
             "qualifier": "Plausibility.HYPOTHETICAL"
         },
         {
             "direction": "pseudo",
             "patterns": [
                 "als baby",
                 "als kind",
                 "als puber",
                 "als tiener",
+                "dd bij",
                 "geduid als",
-                "niet mogelijk"
+                "kan passen bij",
+                "niet mogelijk",
+                "werkdiagnose voor",
+                "waarschijnlijk bij",
+                "onwaarschijnlijk bij",
+                [
+                    {
+                        "TEXT": {
+                            "REGEX": "^\\d+$"
+                        }
+                    },
+                    {
+                        "NORM": "dd"
+                    }
+                ],
+                [
+                    {
+                        "NORM": "dd"
+                    },
+                    {
+                        "TEXT": {
+                            "REGEX": "^\\d+$"
+                        }
+                    }
+                ]
             ],
             "qualifier": "Plausibility.HYPOTHETICAL"
         },
         {
             "direction": "termination",
             "patterns": [
                 "aanwezig",
                 "ter preventie",
-                "zeer waarschijnlijk",
                 "zeker",
                 "zonder twijfel",
                 ","
             ],
             "qualifier": "Plausibility.HYPOTHETICAL"
         },
         {
@@ -827,14 +859,15 @@
                 "als baby",
                 "als kind",
                 "als puber",
                 "als tiener",
                 "bij eerste presentatie",
                 "destijds",
                 "eerdere",
+                "ex-",
                 "gedocumenteerd",
                 "gedocumenteerde",
                 "geschiedenis van",
                 "geschiedenis",
                 "herinnering",
                 "herinneringen",
                 "in de kindertijd",
@@ -895,32 +928,14 @@
                     },
                     {
                         "LOWER": "geleden"
                     }
                 ],
                 [
                     {
-                        "LOWER": "sinds"
-                    },
-                    {
-                        "LOWER": {
-                            "IN": [
-                                "zijn",
-                                "haar"
-                            ]
-                        }
-                    },
-                    {
-                        "TEXT": {
-                            "REGEX": "^\\d{,2}e$"
-                        }
-                    }
-                ],
-                [
-                    {
                         "TEXT": {
                             "REGEX": "^(19|20)\\d{2}$"
                         }
                     }
                 ],
                 [
                     {
@@ -1006,32 +1021,14 @@
                     },
                     {
                         "LOWER": "geleden"
                     }
                 ],
                 [
                     {
-                        "LOWER": "sinds"
-                    },
-                    {
-                        "LOWER": {
-                            "IN": [
-                                "zijn",
-                                "haar"
-                            ]
-                        }
-                    },
-                    {
-                        "TEXT": {
-                            "REGEX": "^\\d{,2}e$"
-                        }
-                    }
-                ],
-                [
-                    {
                         "LOWER": "in"
                     },
                     {
                         "LOWER": {
                             "IN": [
                                 "januari",
                                 "februari",
@@ -1081,27 +1078,125 @@
                 "blanco vg",
                 "blanco voorgeschiedenis",
                 "lijkt meer",
                 "lijkt minder",
                 "lijkt niet meer",
                 "lijkt niet minder",
                 "vg blanco",
-                "voorgeschiedenis blanco"
+                "voorgeschiedenis blanco",
+                [
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "sinds",
+                                "vanaf"
+                            ]
+                        }
+                    },
+                    {
+                        "TEXT": {
+                            "REGEX": "^(19|20)\\d{2}$"
+                        }
+                    }
+                ],
+                [
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "sinds",
+                                "vanaf"
+                            ]
+                        }
+                    },
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "1",
+                                "2",
+                                "3",
+                                "4",
+                                "5",
+                                "6",
+                                "7",
+                                "8",
+                                "9",
+                                "10",
+                                "een",
+                                "twee",
+                                "drie",
+                                "vier",
+                                "vijf",
+                                "zes",
+                                "zeven",
+                                "acht",
+                                "negen",
+                                "tien"
+                            ]
+                        },
+                        "OP": "?"
+                    },
+                    {
+                        "TEXT": {
+                            "IN": [
+                                "jaar",
+                                "jaren",
+                                "maand",
+                                "maanden"
+                            ]
+                        }
+                    }
+                ],
+                [
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "sinds",
+                                "vanaf"
+                            ]
+                        }
+                    },
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "januari",
+                                "februari",
+                                "maart",
+                                "april",
+                                "mei",
+                                "juni",
+                                "juli",
+                                "augustus",
+                                "september",
+                                "oktober",
+                                "november",
+                                "december"
+                            ]
+                        }
+                    },
+                    {
+                        "OP": "?",
+                        "TEXT": {
+                            "REGEX": "^(19|20)\\d{2}$"
+                        }
+                    }
+                ]
             ],
             "qualifier": "Temporality.HISTORICAL"
         },
         {
             "direction": "termination",
             "patterns": [
                 "actueel",
                 "afgenomen",
                 "afname",
                 "nu",
                 "primair",
+                "sinds",
                 "toegenomen",
                 "toename",
+                "vanaf",
                 ","
             ],
             "qualifier": "Temporality.HISTORICAL"
         }
     ]
 }
```

### Comparing `clinlp-0.3.1/clinlp/sentencizer.py` & `clinlp-0.4.0/clinlp/sentencizer.py`

 * *Files identical despite different names*

### Comparing `clinlp-0.3.1/clinlp/util.py` & `clinlp-0.4.0/clinlp/util.py`

 * *Files identical despite different names*

### Comparing `clinlp-0.3.1/pyproject.toml` & `clinlp-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clinlp"
-version = "0.3.1"
+version = "0.4.0"
 description = "Performant and production-ready NLP pipelines for clinical text written in Dutch"
 authors = ["UMCU DIT Analytics <analytics@umcutrecht.nl>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 spacy = "^3.5.3"
```

### Comparing `clinlp-0.3.1/PKG-INFO` & `clinlp-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clinlp
-Version: 0.3.1
+Version: 0.4.0
 Summary: Performant and production-ready NLP pipelines for clinical text written in Dutch
 Author: UMCU DIT Analytics
 Author-email: analytics@umcutrecht.nl
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -70,15 +70,14 @@
 
 text = (
     "Patiente bij mij gezien op spreekuur, omdat zij vorige maand verlies van "
     "reuk na covid infectie aangaf. Zij had geen last meer van kortademigheid, "
     "wel was er nog sprake van hoesten, geen afname vermoeidheid."
 )
 
-
 doc = nlp(text)
 ```
 
 Find information in the doc object:
 
 ```python
 from spacy import displacy
@@ -88,15 +87,15 @@
 
 ![example_doc_render.png](media/example_doc_render.png)
 
 With relevant qualifiers:
 
 ```python
 for ent in doc.ents:
-  print(ent, ent.start, ent.end, ent._.qualifiers)
+  print(ent.start, ent.end, ent, ent._.qualifiers_str)
 
 ```
 
 * `11` `14` `verlies van reuk` `{'Temporality.HISTORICAL'}`
 * `25` `26` `kortademigheid` `{'Negation.NEGATED'}`
 * `33` `34` `hoesten` `{}`
 * `37` `38` `vermoeidheid` `{}`
@@ -132,15 +131,15 @@
 - Regarding [DEDUCE](https://github.com/vmenger/deduce) tags as a single token (e.g. `[DATUM-1]`). 
   - Deidentification is not builtin `clinlp` and should be done as a preprocessing step.
 
 ### Normalizer
 
 The normalizer sets the `token.norm` attribute, which can be used by further components (entity recognition, qualification) for matching. It currently has two options (enabled by default):
 - Lowercasing
-- Removing diacritings, where possible. For instance, it will map `ë` `->` `e`, but keeps most other non-ascii characters intact (e.g. `µ`, `²`).
+- Removing diacritics, where possible. For instance, it will map `ë` `->` `e`, but keeps most other non-ascii characters intact (e.g. `µ`, `²`).
 
 Note that this component only has effect when explicitly configuring successor components to match on the `token.norm` attribute. 
 
 ### Sentence splitter
 
 The sentence splitter can be added as follows:
 
@@ -148,17 +147,17 @@
 nlp.add_pipe('clinlp_sentencizer')
 ```
 
 It is designed to detect sentence boundaries in clinical text, whenever a character that demarks a sentence ending is matched (e.g. newline, period, question mark). It also correctly detects items in an enumerations (e.g. starting with `-` or `*`). 
 
 ### Entity matcher
 
-Currently, the spaCy builtin `PhraseMatcher` and `Matcher` can be used for finding (named) entities in text. The first one accepts literal phrases only, that are matched in the tokenized text, while the second one also accepts [spaCy patterns](https://spacy.io/usage/rule-based-matching#adding-patterns). These are not tailored for the clinical domain, but nevertheless useful when a somewhat coherent list of relevant patterns can be generated/obtained.
+Currently, the spaCy builtin `EntityRuler` can be used for finding (named) entities in text. It accepts both literal phrases (single terms or multi-word expressions) and [spaCy patterns](https://spacy.io/usage/rule-based-matching#adding-patterns), which give more control over the specific sequence of tokens to match. The spaCy `EntityRuler` is not necessarily tailored for the clinical domain, but nevertheless useful when a somewhat coherent list of relevant patterns can be generated/obtained. A better or more specific NER module will hopefully be added in the future. 
 
-For instance, a matcher that helps recognize COVID19 symptoms:
+For instance, a matcher that helps recognize COVID-19 symptoms:
 
 ```python
 ruler = nlp.add_pipe('entity_ruler', config={'phrase_matcher_attr': "NORM"})
 
 terms = {
     'covid_19_symptomen': [
         'verkouden', 'neusverkouden', 'loopneus', 'niezen', 
@@ -168,27 +167,26 @@
 }
 
 for term_description, terms in terms.items():
     ruler.add_patterns([{'label': term_description, 'pattern': term} for term in terms])
 ```
 
 For more info, it's useful to check out these spaCy documentation pages:
+* [[spaCy API] EntityRuler](https://spacy.io/api/entityruler)
 * [Rule based matching](https://spacy.io/usage/rule-based-matching)
-* [[spaCy API] Matcher](https://spacy.io/api/matcher)
-* [[spaCy API] PhraseMatcher](https://spacy.io/api/phrasematcher)
 
-Note that the `DependencyMatcher` cannot be used, and neither are part of speech tags available, as no good models for determining this information for clinical text exist (yet).  
+Note that Part of Speech tags and dependency trees and cannot be used in `clinlp`, as no good models for determining this information for clinical text exist (yet).  
 
 ### Qualifier detection
 
-After finding entities, it's often useful to qualify these entities, e.g.: are they negated or affirmed, historical or current? `clinlp` currently implements the rule-based [Context algorithm](https://doi.org/10.1016%2Fj.jbi.2009.05.002), and a [transformer-based negation detector](https://doi.org/10.48550/arxiv.2209.00470). 
+After finding entities, it's often useful to qualify these entities, e.g.: are they negated or affirmed, historical or current? `clinlp` currently implements two options: the rule-based Context Algorithm, and a transformer-based negation detector. 
 
 #### Context Algorithm
 
-The rule-based Context Algorithm is fairly accurate, and quite transparent and fast. A set of rules, that checks for negation, temporality, plausibility and experiencer, is loaded by default:
+The rule-based [Context Algorithm](https://doi.org/10.1016%2Fj.jbi.2009.05.002) is fairly accurate, and quite transparent and fast. A set of rules, that checks for negation, temporality, plausibility and experiencer, is loaded by default:
 
 ```python
 nlp.add_pipe('clinlp_context_algorithm', config={'phrase_matcher_attr': 'NORM'})
 ```
 
 A custom set of rules, including different types of qualifiers, can easily be defined. See [`clinlp/resources/psynlp_context_rules.json`](clinlp/resources/psynlp_context_rules.json) for an example, and load it as follows:
```

