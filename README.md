# Intermediate evaluation on RDF, RDFS

## Subject

*Work in pairs*

<ul>
  <li>Synthesis on RDF/RDFS, 3 pages maximum, in pdf format. What did you learn? What are the principles of the model? What are the key elements of the language? What are the best modelling practices? </li>
  <li>RDF database describing (last year) students and the organization of their curriculum within Polytech Nice Sophia.
    <ul>
      <li>Describe each student in a separate RDF graph, stored in a file studentName.ttl. You should provide the full description of yourself.</li>
      <li>Describe the organization of the curriculum in one or several other separate RDF graphs, stored in a file Polytech.ttl. or files Polytech_xxx.ttl. It should describe the organization of mineures, their obligatory and optional courses, the teachers managing or involved in courses and mineures, the student delegates, etc. You should focus on the description of your own mineure, but mention the others.</li>
      <li>Describe your model in at least two RDFS vocabularies, stored in files model_xxx.ttl. </li>
      <li>Provide a screenshot of one of your RDF graphs produced by the W3C validator</li>
      <li>Provide a screenshot of one of your RDFS graph produced by the W3C validator</li>
      <li>an HTML page presenting yourself (like an online CV but don't spend time to make it look good if you don't already have one) containing RDF metadata in RDFa format</li>
      <li>a file containing your RDF description in JSON-LD</li>
    </ul>
  </li>
</ul>

You must upload a single zip file containing your entire work.
## Description

Dans <b>model_scolarity.ttl</b> et <b>model_organisation.ttl</b>, on créer les classes et les propriétés nécessaires à la description d'une école du réseau Polytech. 
<ul>
  <li><b>model_scolarity.ttl</b> : Focus sur les personnes composants l'école, les élèves et les professeur.</li>
  <li><b>model_organisation.ttl</b> : Focus sur les filières (Major et Minor) et la classe Course pour décrire les cours disponibles à Polytech</li>
</ul>
Ces schémas forment le vocabulaire utiliser ensuite pour créer des instances de Professeurs, d'élève, de cours ... La création de ces instances à lieu dans les fichiers <b>Polytech_scolarity.ttl</b> et <b>Polytech_organisation.ttl</b> .
<ul>
  <li><b>Polytech_scolarity.ttl</b> : Focus sur la creation des professeur (Teacher) et des élèves délégué de filières </li>
  <li><b>Polytech_organisation.ttl</b> : Focus sur la creation des filière majeur et mineurs ainsi que les cours qui les composes</li>
</ul>
Dans ces deux fichiers, on traite précisement uniquement de nos filières IHM et SD. Les informations sur nous deux (Gaymard Erwan et Barthélemy Passin-Cauneau) sont stockées dans <b>studentGaymard.ttl</b> et <b>studentPassinCauneau.ttl</b>.

## Workflow

On utilise les outils suivants pour valider et visualiser notre code RDF.

Turtle Validator      : http://ttl.summerofcode.be/ <br>
RDF Converter         : https://www.easyrdf.org/converter <br>
Visualization RDF/XML : https://www.w3.org/RDF/Validator/rdfval

Ressources utiles sur RDF : <br>
https://www.w3.org/TR/rdf-schema/#ch_classes <br>

