# Identifiers

As you write a Java program, you need to create and use _identifiers_. These are the names of things that you create inside your program. Everything you create has a name, so everything you create has an identifier.

## The rules for identifiers are simple:

* You must start each identifier with a letter, underscore or a dollar sign
* After the first character, you can use any combination of letters, underscores, dollar signs or digits
* Don't use Java Keywords
* Java is case sensitive so InvoiceTotal and invoiceTotal are considered different identifiers

## Valid Identifiers

| **Valid** | **Invalid** |
| :--- | :--- |
| `InvoiceApp` | `Invoice App` |
| `InvoiceApp2` | `public` |
| `TITLE` | `@TITLE` |
| `$orderTotal` | `!orderTotal` |
| `_orderTotal` | `true` |
| `input_string` | `87` |
| `subtotal` | `67g3` |
| `_get_total` | `return` |
| `MONTHS_PER_YEAR` | `null` |
| `bhy56jkls_$` | `64_valid` |

## Keywords

* The Java programming language has total of 50 reserved keywords which have special meaning for the compiler and cannot be used as variable names. 

\|boolean\|if\|interface\|class\|true\| \|char\|else\|package\|volatile\|false\| \|byte\|final\|switch\|while\|throws\| \|float\|private\|case\|return\|native\| \|void\|protected\|break\|throw\|implements\| \|short\|public\|default\|try\|import\| \|double\|static\|for\|catch\|synchronized\| \|int\|new\|continue\|finally\|const\| \|long\|this\|do\|transient\|goto\| \|abstract\|super\|extends\|instanceof\|null\|

* An **identifier** is a name you create in your Java program. Identifiers can be the names of classes, methods, variables and more.
* A **keyword** is a word that's reserved for use by  Java. You can't a keyword as an identifier.
* Java is case-sensitive. When you refer to an identifier use the same case as when you define it. \* You may see Java programmers create identifiers that are the same as class names but differ only in case. This looks confusing but it is actually correct. We recommend you not do this.

