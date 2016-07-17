# INSTS

A list of institutions and jdCollege tags for use with the allowed_colleges config Set.

Code works by mixing together the institutions and colleges from the lookup request. As such, if you really don't like DAMTP, but a friend of yours attends both it and Christ's, you can't exclude them by including Christ's but not DAMTP.

## Colleges

A list of all of the institution ids returned by the ibisclient interfacing with the University Lookup Service.

Fellows & Staff at colleges are included under 'All Members of'. Thus, if you want to grant access to Christ's Postgraduates only:
```python
c.RavenAuthenticator.allowed_colleges = {'CHRISTSPG'}
```

| College | Institution ID | Description
Christ's College | CHRISTS | All Members of Christ's College
| CHRSTPG | Postgraduates Only
| CHRSTUG | Undergraduates Only
Churchill College | CHURCH | All Members of Churchill College
| CHURPG | Postgraduates Only
| CHURUG | Undegraduates Only
Clare College | CLARE | All Members of Clare College
| CLAREPG | Postgraduates Only
| CLAGEUG | Undergraduates Only
Clare Hall | CLAREH | All Members of Clare Hall
| CLARHPG | Postgraduates Only
Corpus Christi College | CORPUS | All Members of Corpus Christi College
| CORPPG | Postgraduates Only
| COPUG | Undergraduates Only
Darwin College | DARWIN | All Members of Darwin College
| DARPG | Postgraduates Only
Downing College | DOWN | All Members of Downing College
| DOWNPG | Postgraduates Only
| DOWNUG | Undergraduates Only
Emmanuel College | EMM | All Members of Emmanuel College
| EMMPG | Postgraduates Only
| EMMUG | Undergraduates Only
Fitzwilliam College | FITZ | All Members of Fitzwilliam College
| FITZPG | Postgraduates Only 
| FITZUG | Undergraduates Only
Girton College | GIRTON | All Members of Girton College
| GIRTPG | Postgraduates Only
| GIRTUG | Undergraduates Only
Gonville & Caius College | CAIUS | All Members of Gonville & Caius College
| CAIUSPG | Postgraduates Only
| CAIUSUG | Undergraduates Only
Homerton College | HOM | All Members of Homerton College
| HOMPG | Postgraduates Only
| HOMUG | Undergraduates Only
Hughes Hall | HUGHES | All Members of Hughes Hall
| HUGHPG | Postgraduates Only
| HUGHUG | Undergraduates Only
Jesus College | JESUS | All Members of Jesus College
| JESUSPG | Postgraduates Only
| JESUSUG | Undergraduates Only
King's College | KINGS | All Members of King's College
| KINGSPG | Postgraduates Only
| KINGSUG | Undergraduates Only
Lucy Cavendish College | LCC | All Members of Lucy Cavendish College
| LCCPG | Postgraduates Only
| LCCUG | Undergraduates Only
Magdalene College | MAGD | All Members of Magdalene College
| MAGDPG | Postgraduates Only
| MAGDUG | Undergraduates Only
Murray Edwards College | NEWH | All Members of Murray Edwards College
| NEWHPG | Postgraduates Only
| NEWHUG | Undergraduates Only
Newnham College | NEWN | All Members of Newnham College
| NEWNPG | Postgraduates Only
| NEWNUG | Undergraduates Only
Pembroke College | PEMB | All Members of Pembroke College
| PEMBPG | Postgraduates Only
| PEMBUG | Undergraduates Only
Peterhouse | PET | All Members of Peterhouse
| PETPG | Postgraduates Only
| PETUG | Undergraduates Only
Queens' College | QUEENS | All Members of Queens' College
| QUENPG | Postgraduates Only
| QUENUG | Undergraduates Only
Robinson College | ROBIN | All Members of Robinson College
| ROBINPG | Postgraduates Only
| ROBINUG | Undergraduates Only
Selwyn College | SEL | All Members of Selywn College
| SIDPG | Postgraduates Only
| SIDUG | Undergraduates Only
St Catharine's College | CATH | All Members of St Catharine's College
| CATHPG | Postgraduates Only
| CATHUG | Undergraduates Only
St Edmund's College | EDMUND | All Members of St Edmund's College
| EDMPG | Postgraduates Only
| EDMUG | Undergraduates Only
St John's College | JOHNS | All Members of St John's College
| JOHNSPG | Postgraduates Only
| JOHNSUG | Undergraduates Only
Trinity College | TRIN | All Members of Trinity College
| TRINPG | Postgraduates Only
| TRINUG | Undergraduates Only
Trinity Hall | TRINH | All Members of Trinity Hall
| TRINHPG | Postgraduates Only
| TRINHUG | Undergraduates Only
Wolfson College | WOLFC | All Members of Wolfson College
| WOLFCPG | Postgraduates Only
| WOLFCUG | Undergraduates Only

## Institutions

By no means a complete list.

| Institution | Institution ID |
| Cambridge Computational Biology Institute | CCBI
| Computer Laboratory | CL |
| Department of Applied Maths and Theoretical Physics | DAMTP |
| Department of Biochemistry | BIOCH |
| Department of Chemical Engineering and Biotechnology | CEB |
| Department of Chemistry | CHEM |
| Department of Earth Sciences | EARTH |
| Department of Engineering | ENG |
| Department of Genetics | GEN |
| Department of Geography | GEOG |
| Department of Materials Science and Metallurgy | MET |
| Department of Oncology | RADT |
| Department of Pathology | PATH |
| Department of Pharmacology | PHARM |
| Department of Physics | PHY |
| Department of Physiology, Development and Neuroscience | PHSI |
| Department of Radiology | RADIOL |
| Department of Veterinary Medicine | CVM |
| Department of Zoology | ZOO |
| Faculty of Economics | ECON |
| Sanger Centre | SANGRES |




