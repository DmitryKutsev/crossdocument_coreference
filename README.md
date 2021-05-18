
# Извлечение кросс-текстовой анафоры из русскоязычного пользовательского контента в медицинской сфере.

# Cross-document anaphora extraction from medicine-related content generated by Russian users.

## Вступление.

Извлечение данных из пользовательского медицинского контента - важная задача,
позволяющая решить, или упростить решение для множества задач в медицине. Такие
задачи, как извлечение отзывов, и иной информации о препаратах, или проведение
диагностики на имеющихся данных о лечении заболеваний, дополняют методики лечения.
На основе обработанных данных составляются рекомендательные и консалтинговые
системы, помогающие врачам поставить диагноз, или подобрать наиболее подходящий
препарат.
Разрешение анафоры - важная составляющая для большинства систем извлечения
данных из текстов. Анафора - зависимость между интерпретацией какой-то
одной сущности в тексте от другой, встретившейся в том же тексте ранее.
Упоминание, встретившееся первым, называют антецедентом, а следующее за ним
упоминание того же объекта - анафором. Отношения между антецедентом и анафором
можно назвать кореферентными.
Например:
“А кто принимал респеридон расскажите плз как у вас с либидо, было ли сильное
снижение или нет? А также очень интересно как влияет он на депрессивную
составляющую..?”
Здесь местоимение “он” является анафором, и ссылается на антецедент, респеридон.

Нахождение кореференциальных связей может применяться также во множестве систем,
помимо медицинских. Например, системы машинного перевода, извлечение
именованных сущностей, классификация событий, и многие другие задачи могут
использовать в своих алгоритмах разрешение анафоры.


## Типы анафоры и процесс разрешения.

Самый распостраненный тип анафоры подразумевает связи местоимения(реже существительного) с именованной сущностью, 
или упоминанием этой сущности. Такой тип анафоры называют прономинальной.

Существуют связи, в которых и анафор, и антецедент являются существительными(или, в некоторых случаях, именными группами существительного), например:
“Знаю, что тиапридал применяется при алкоголизме для купирования агрессивности.
Есть ли у кого-нибудь опыт применения этого препарата у пожилых людей?”

Различают также анафоры, находящиеся внутри одного предложения, и анафоры, члены
которых находятся в разных предложениях(интрасентенциальные, и
интерсентенциальные).

В основном в системах разрешения анафоры в качестве анафора рассматривают только именные группы существительных. Хотя бывают случаи,
когда в качестве антецедента выступают глагольные группы, целые предложения, или участки дискурса[1]. Также большинство исследований рассматривает анафоры с кореферентными связями в пределах нескольких предложений одного текста. 
Сами системы разрешения анафоры можно разделить на правиловые системы [5], системы на основе алгоритмов машинного обучения[7, 8], и гибридные системы[3].
Правиловые системы отбирают подходящих кандидатов в антецеденты на основании допусков и ограничений, например:
  - Согласование по гендеру и числу.
...













-----
[1] http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.29.6235&rep=rep1&type=pdf
ANAPHORA RESOLUTION: THE STATE OF THE ART, Ruslan Mitkov

Hirst, Graeme. 1981.Anaphora in natural language understanding. Berlin Springer Verlag,
1981.

[2] https://www.aclweb.org/anthology/W16-0711.pdf
Error analysis for anaphora resolution in Russian: new challenging issues
for anaphora resolution task in a morphologically rich language
Svetlana Toldova Ilya Azerkovich Anna Roytberg

[3] http://www.dialog-21.ru/media/3913/gureenkovaoaetal.pdf
Complex Approach towards
Algoritm Learning for Anaphora
Resolution in Russian Language
Gureenkova O. A.,
Batura T. V. ,
Kozlova A. A.,
Svischev A. N.

[4] https://arxiv.org/pdf/1805.10163.pdf
Context-Aware Neural Machine Translation Learns Anaphora Resolution
Elena Voita
University of Amsterdam, Netherlands
Pavel Serdyukov
Rico Sennrich

[5] http://www.dialog-21.ru/media/4829/inshakovaes-167.pdf
AN ANAPHORA RESOLUTION SYSTEM FOR RUSSIAN BASED ON ETAP-4 LINGUISTIC PROCESSOR1 Inshakova E. S

[6] https://www.aclweb.org/anthology/J13-4004.pdf
Jurafsky D., Lee H., Chang A., Peirsman Y., Chambers N., Surdeanu M. (2013), Deterministic Coreference Resolution Based on Entity-Centric, Precision-Ranked
Rules, Association for Computational Linguistics, Vol. 39, N 4, pp. 885–916.


[7] http://www.dialog-21.ru/digests/dialog2014/materials/pdf/Kamenskaya%D0%9C%D0%90.pdf
Kamenskaya М. А., Khramoin I. V., Smirnov I. V. (2014), Data-driven Methods
for Anaphora Resolution of Russian, Computational Linguistics and Intellectual Technologies: Papers from the Annual International Conference “Dialogue”
(2014), Issue 13 (20), pp. 241–250.

http://www.dialog-21.ru/digests/dialog2014/materials/pdf/ProtopopovaEV.pdf
[8] Protopopova E. V., Bodrova A. A., Volskaya S. A., Krylova I. V., Chuchunkov A. S.,
Alexeeva S. V., Bocharov V. V., Granovsky D. V. (2014), Anaphoric Annotation and
Corpus-Based Anaphora Resolution: An Experiment, Computational Linguistics
and Intellectual Technologies: Papers from the Annual International Conference
“Dialogue” (2014), Issue 13 (20), pp. 562–571
