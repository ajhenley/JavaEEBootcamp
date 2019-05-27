# JavaServer Pages Standard Tag Library \(JSTL\)

> JSTL extends the JSP specification by adding a tag library of JSP tags for common tasks such as conditional execution, loops and internationalization.

The JavaServer Pages Standard Tag Library \(JSTL\) is a collection of four custom-tag libraries which extend the JSP specification. The JSTL is a component of the Java EE Web application development platform.

## Usage of JSTL 1.1

As for the use of JSTL 1.1 the JSP-EL is required, a servlet-container has to be conform to at least the JSP-2.0 specifications in order to be be used on this. The reference implimentation is made up of two JAR – archives **standard.jar** and **jstl.jar**. In most containers they usually need to be located in the lib-path of the web application only. To ensure backwards compatibility the JSTL 1.1 is referenced by the URI [http://java.sun.com/jsp/jstl/fmt](http://java.sun.com/jsp/jstl/fmt) whereas [http://java.sun.com/jstl/fmt](http://java.sun.com/jstl/fmt) is used for JSTL 1.0.

## Example JSP-page in XML-notation \(JSPX\):

## Code-Explanations:

In the `jsp:root` – element the usage of the basis- und the I18N-Taglibs \(core and fmt\) from the JSTL is indicated and linked to the according XML-namespace. Under the headline ''Iteration'' the ''forEach-Tag'' from the core-library is used: It displays the tag-body \(i.e., the content of the Tag\) ten times. In this loop with ''`${num}`'' you can find JSP – Expression. With every loop cycle the current data from ''num'' is displayed here. Under the headline ''Formatting'' the ''formatNumber''-tag from the fmt – library of JSTL is used. Depending on the adjusted lanuage \(this can be set by fmt:setLocale for example\) the number 10000 will be formated \(e.g. in german as „EUR 10.000,00“ and in english as „EUR 10,000.00“\)

