---
layout: default
title: Architectural Decision Records (ADRs)
toc: true
source: https://github.com/adr/adr.github.io/blob/main/index.md
---

> **Примітка перекладача:** Це переклад офіційної вступної статті з екосистеми [adr.github.io](https://github.com/adr/adr.github.io/blob/main/index.md).

## Мотивація та Визначення

[Архітектурне рішення (AD)](https://en.wikipedia.org/wiki/Architectural_decision) — це обґрунтований проєктний вибір, який відповідає архітектурно значущій функціональній чи нефункціональній вимозі.
[Архітектурно значуща вимога (ASR)](https://en.wikipedia.org/wiki/Architecturally_significant_requirements) — це вимога, яка має вимірюваний вплив на архітектуру та якість програмної та/або апаратної системи.
*Запис архітектурного рішення (Architectural Decision Record, ADR)* фіксує одне окреме AD та його обґрунтування.
Простими словами, ADR допомагає зрозуміти причини ухвалення обраного архітектурного рішення, а також пов'язані з ним компроміси та наслідки.
Сукупність ADR, створених та підтримуваних у проєкті, утворює його *журнал рішень (decision log)*.
Усе це належить до сфери управління архітектурними знаннями (Architectural Knowledge Management, AKM), проте використання ADR може бути поширене на дизайн та інші рішення («будь-який запис рішення»).

Метою [організації GitHub adr](https://github.com/adr) є:

1. Обґрунтування необхідності та переваг фіксації AD, а також встановлення спільного словника термінів.
2. Посилення екосистеми інструментів навколо ADR на підтримку agile-практик, а також ітеративних та інкрементальних інженерних процесів.
3. Надання посилань на загальнодоступні знання в контексті AKM та ADR.

## ADR у ЗМІ та Публікаціях

- (німецькою) [Architekturentscheidungen sichtbar und nachvollziehbar gestalten](assets/2026-03-10%20-%20ADR%2C%20MADR%2C%20eADR%20-%20JavaLand%202026.pdf) на конференції [JavaLand 2026](https://www.javaland.eu/) (2026-03-10).
- [Azure Well-Architected Framework](https://learn.microsoft.com/en-us/azure/well-architected/architect-role/architecture-decision-record) висвітлює використання ADR та цей вебсайт (2024-11-10).
- [Love Unrequited: The Story of Architecture, Agile, and How Architecture Decision Records Brought Them Together](https://ieeexplore.ieee.org/document/9801811), Майкл Кілінг (Michael Keeling) у колонці Pragmatic Designer журналу IEEE Software (Випуск 39, № 4, 2022) ([PDF](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9801811)).
- Фіксація архітектурних рішень позиціонується як одна з ключових дій у [Design Practice Reference](https://leanpub.com/dpr), електронній книзі на LeanPub.
- Розділ 3 книги ["Patterns for API Design: Simplifying Integration with Loosely Coupled Message Exchanges"](https://api-patterns.org/book/) серії Addison Wesley Signature Series від Pearson містить шість історій, що супроводжують концептуальний рівень проєктування API: 29 повторюваних рішень з варіантами та критеріями. Дізнайтеся більше в цьому [блозі](https://medium.com/nerd-for-tech/api-patterns-website-redesigned-and-sample-book-chapter-available-df9daf4b5e15).
- (німецькою) [Gut dokumentiert: Architecture Decision Records](https://www.heise.de/hintergrund/Gut-dokumentiert-Architecture-Decision-Records-4664988.html) за авторством [@obfischer](https://github.com/obfischer), опубліковано на [heise online](https://www.heise.de/).

## Довідкова Інформація

Робота в організації adr базується на настановах та принципах з праці [Sustainable Architectural Decisions](https://www.infoq.com/articles/sustainable-architectural-design-decisions) Здуна та ін. (Zdun et al.), зокрема на форматі Y-statement, запропонованому в цій статті.

Більш загальну довідкову інформацію та рекомендації щодо ADR можна знайти в наступних джерелах:

- Порівняння семи шаблонів наведено у виступі на конференції WICSA 2015: ["Architectural Decision Guidance Across Projects --- Problem Space Modeling, Decision Backlog Management and Cloud Computing Knowledge"](https://www.ost.ch/fileadmin/dateiliste/3_forschung_dienstleistung/institute/ifs/cloud-application-lab/admentor-wicsa2015ubmissionv11nc.pdf).
- [Architectural Decisions — The Making Of](https://www.ozimmer.ch/practices/2020/04/27/ArchitectureDecisionMaking.html) описує історію запису архітектурних рішень з кінця 1990-х років, а також містить приклади та настанови щодо обґрунтування рішень.
- [Documenting Architecture Decisions](https://cognitect.com/blog/2011/11/15/documenting-architecture-decisions.html) — це стаття в блозі Майкла Найгарда (Michael Nygard) за 2011 рік, яка популяризувала цей концепт.
- [Architectural Decision Records (ADR): Open & Transparent Decision History](https://openpracticelibrary.com/practice/architectural-decision-records-adr/) — практика в Open Practice Library.
- AWS Prescriptive Guidance рекомендує [використовувати записи архітектурних рішень для оптимізації технічного прийняття рішень у проєктах розробки програмного забезпечення](https://docs.aws.amazon.com/prescriptive-guidance/latest/architectural-decision-records/introduction.html).
- [Architecture Decision Records in Action by Michael Keeling (IBM Watson Group) and Joe Runde (IBM) [YouTube]](https://www.youtube.com/watch?v=41NVge3_cYo) — презентація, що містить емпіричні показники.
- [ADRs and Architecture Stories](https://www.developertoarchitect.com/lessons/lesson168.html) є частиною відеосерії Марка Річардса (Mark Richards), де пояснюються ADR на основі шаблону Найгарда.
- Додаткові посилання та ресурси можна знайти на вебсторінці [Управління архітектурними знаннями (AKM)](https://www.ost.ch/en/research-and-consulting-services/computer-science/ifs-institute-for-software-new/cloud-application-lab/architectural-knowledge-management-akm).
