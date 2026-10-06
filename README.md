# xslt2-parse-alarm-log
Using XSLT2 to parse an XML clinical audit log file from PICiX C.03. The XML log file in English contains fields Date, Institution, Bed_x0020_Label, Action, Device_x0020_Name, Clinical_x0020_User and Action_x0020_Type. The x0020 in the names goes away in PICiX 4. 

XSLT2 requires Saxon-HE 10.5J from Saxonica and Java to parse. 

To execute:

java -cp c:\saxon\SaxonHE10-5J\saxon-he-10.5.jar net.sf.saxon.Transform -t -s:"c:\saxon\XSLT parse\test.xml" -xsl:"c:\saxon\XSLT parse\parseXSLT2-en.xslt" -o:"c:\saxon\XSLT parse\test.csv"
