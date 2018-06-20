A ontologia aqui proposta, CASE-DUL, consiste em um alinhamento entre as ontologias CASE (Cyber-investigation Analysis Standard Expression) e DUL (DOLCE+DnS Ultralite).

A ontologia CASE foi copiada de https://github.com/ucoProject/CASE/blob/master/case.ttl e foi modificada para que a URI da ontologia apontasse para uma URL existente: a versão original aponta para http://case.example.org/core e a vesão alterada aponta para https://raw.githubusercontent.com/atilaromero/CASE-DUL/master/case.ttl.

Uma cópia da ontologia DUL foi obtida de http://www.ontologydesignpatterns.org/ont/dul/DUL.owl e salva no repositório https://github.com/atilaromero/CASE-DUL.

Uma terceira ontologia, CASE-DUL, foi criada para especificar o alinhamento entre as duas primeiras.

Para isso, o primeiro passo foi fazer uma referência do tipo owl:Import na CASE-DUL para a CASE e para a DUL.

Na ontologia CASE, as classes e subclasses de Enumeration, OrderedList, PropertyBundle, Slot, e SupportingClasses não participaram do alinhamento, pois são as subclasses de UcoObject que contém os conceitos principais a serem alinhados.

O alinhamento em si foi simples e consistiu em identificar quais classes da ontologia CASE possuiam classe superior ou equivalente na ontologia DUL.

Os seguintes alinhamentos foram identificados:
 - Action-Action
 - ActionLifecycle-Task
 - Location-PhysicalPlace
 - Role-Role
