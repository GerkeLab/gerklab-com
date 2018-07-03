---
title: '{{ replace .TranslationBaseName "-" " " | title }}'
author:
  - Author One
  - Author Two
  - Author Three
date: {{ .Date }}
published_in: "Journal of Publication"
doi: 
links:
  - name: link name (repeat sections as needed)
    url: '#'
  - name: link name (repeat sections as needed)
    url: '#'
header_buttons:
  - url: "#"
    text: Button Text
    class: primary # primary|secondary|info + [outline]
    icon: ai ai-biorxiv # Academic Icons or Font Awesome icon code
  - url: "#"
    text: Button Text
    class: primary # primary|secondary|info + [outline]
    icon: ai ai-biorxiv # Academic Icons or Font Awesome icon code
description: "This description appears in the publications list and as a callout in the publication page."
citation: "Authors. Formatted Citation. Journal. Identifiers. etc."
abstract: |
    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nemo nostrum istius generis asotos iucunde putat vivere. Septem autem illi non suo, sed populorum suffragio omnium nominati sunt. Falli igitur possumus. Praeteritis, inquit, gaudeo. _Dici enim nihil potest verius._ Duo Reges: constructio interrete. Indicant pueri, in quibus ut in speculis natura cernitur.

    Isto modo ne improbos quidem, si essent boni viri. Qualem igitur hominem natura inchoavit? `Sed ad rem redeamus;` Quodsi ipsam honestatem undique pertectam atque absolutam.

    Quorum sine causa fieri nihil putandum est. Nam, ut sint illa vendibiliora, haec uberiora certe sunt. Non quam nostram quidem, inquit Pomponius iocans; Quae cum dixisset paulumque institisset, Quid est? Ut necesse sit omnium rerum, quae natura vigeant, similem esse finem, non eundemnquam, faciam. **Quamquam te quidem video minime esse deterritum.** `Egone quaeris, inquit, quid sentiam?` Hic ego: Pomponius quidem, inquam, noster iocari videtur, et fortasse suo iure. **Cur deinde Metrodori liberos commendas?**
---

<!--
## Common icons

Font Awesome: https://fontawesome.com/icons
Academic Icons: http://jpswalsh.github.io/academicons/

github: fab fa-github
twitter: fab fa-twitter
rocket (app): fas fa-rocket
biorxiv: ai ai-biorxiv
arvix: ai ai-arxiv
doi: ai ai-doi
pubmed: ai ai-pubmed
generic paper: far fa-file-alt
generic project: fas fa-briefcase
-->

<!--
You can include extra content here as markdown.
It will render after Abstract and Links and before Citation.
-->