---
layout: default
title: How do I add content to the Open Government Portal? (draft)
lang: en
altLang: fr
altLangPage: publier-contenu
collectionDirectory: views-vues/open-gov-gouv-ouvert
step1:
  title: "Step 1: Determine whether the content is of business value"
  q1Label: Does the content help explain who you are? (For example, does it outline what your department or agency does, explain its constitutional and legal governance, provide a list of contacts or indicate where it is located?)
  q2Label: Is the content about the programs or services you offer? (For example, does it describe services offered? Does it contain advice and guidance? Does it include publications or media releases, administrative data, or information about transactions or grants and contributions?)
  q3Label: Is the content about your finances, what you spend and how you spend it? (For example, does it include projected and actual income and expenditures, or annual Minister's office expenses? Does it relate to tendering, procurement and contracts, travel and hospitality, or position reclassifications?)
  q4Label: Is the content about your priorities and how you're doing at achieving them? (For example, does it include assessments and reviews, ministerial mandate letters, or reports tabled in Parliament?)
  q5Label: Is the content about your policies and procedures? (For example, does it explain how you fulfill your responsibilities? Does it contain policy proposals and announcements? Does it include updates on decision-making processes and consultations?)
  q6Label: Is the content about your lists and registers that your organization is responsible for? (For example, is it about lists or registers required by legislation or relating to your functions? Does it include summaries of complete Access to Information requests?)
  q7Label: Will the content benefit Canadians either by improving services or by promoting innovation and economic growth?
  q8Label: Has the content been frequently requested through access to information requests?
  q9Label: Will the content help the public better understand Government of Canada priorities and commitments?
  q10Label: Will the content help other Government of Canada institutions provide more effective services?
  q11Label: Does the content provide information of value to researchers, students, academics or interested citizens?
  failTitle: Cannot be released
  failBody: Based on your answers, the content cannot be released as is.
step2:
  title: "Step 2: Determine whether the content is subject to restrictions"
  q1Label: Does the content include classified or protected information?
  q2Label1: Does the content include any of the following personal information
  q2Label2: about an individual?
  q2Sub1Label: a. race
  q2Sub2Label: b. national or ethnic origin
  q2Sub3Label: c. religion
  q2Sub4Label: d. age
  q2Sub5Label: e. marital status
  q2Sub6Label: f. medical, criminal or employment history status
  failTitle: Subject to restrictions
  failBody: Based on your last answer, the content is subject to restrictions, so it is not ready for release.
step3:
  title: "Step 3: Determine whether the content is ready for release"
  q1Label1: Is the content available in an accessible format that meets the requirements of the
  q1LabelLinkText: Standard on Web Accessibility
  q1LabelLinkURL: https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=23601
  q1Label2: (For example, CSV, XML, HTML, PDF/UA)
  q2Label: Is the content in both official languages?
  q3Label: Can the content be released under the
  q3LabelLinkText: Open Government Licence
  q3LabelURL: https://open.canada.ca/en/open-government-licence-canada
  q4Label: Has the content been assessed and verified for quality? (For example, completeness, accuracy, timeliness, consistency)
  q5Label: Has a data dictionary been developed to describe elements in the content?
  q6Label: Has the chief information officer or the information management senior offical approved the release of the content?
  failTitle: Not ready for release
  failBody: Based on your last answer, content is not ready for release.
fail:
  help1: For information on what changes are needed so that your content can be released
  helpConsult: consult the
  helpOr: or
  helpContact: contact
guidebook:
  linkText: Open Government Guidebook
  url: "https://open.canada.ca/ckan/en/dataset/9eaa6d0e-4b8c-5241-acf7-c6885294b8c1"
contactEmail: open-ouvert@tbs-scgt.gc.ca
---
{% assign dataVariable = site.playbookData[page.lang] %}{%
assign dataSource = site.data[dataVariable] %}

In accordance with the [Directive on Open Government](https://www.tbs-sct.gc.ca/pol/doc-eng.aspx?id=28108), the Government of Canada is committed to maximizing the release of government information and data of business value to support transparency, accountability, citizen engagement, and socio-economic benefits.

This page will help you decide whether to release content, either a dataset (structured information) or an information asset (unstructured information), on open.canada.ca.

This process has 3 steps:

- Step 1: Determine whether the content is of business value
- Step 2: Determine whether the content is subject to restrictions
- Step 3: Determine whether the content is ready for release

{% include views-vues/open-gov-gouv-ouvert/release-content-publier-contenu-questionnaire.html %}

<!-- No questions to answer, just instructions for releasing the content on open.canada.ca. -->
<section id="step4-section" class="hidden">

<div class="panel panel-success">
<header class="panel-heading">
<h2 class="panel-title">Your content is ready for release on open.canada.ca</h2>
</header>
<div class="panel-body">

Your content is ready to be released on [open.canada.ca](https://open.canada.ca), you will need to:

- Create a metadata record describing the content on the Open Government Registry: The [Open Government Registry Guide](https://open.canada.ca/ckan/en/dataset/c2529700-2728-5c39-9107-1102e9cfb7bb) explains how to create this record.
- Send an email to <{{ page.contactEmail }}> to ask that the metadata record be reviewed and released on [open.canada.ca](https://open.canada.ca).
- Release the content: The [{{ page.guidebook.linkText }}]({{ page.guidebook.url }}) explains how to release your content on [open.canada.ca](https://open.canada.ca).

For more information, please contact the Open Government group at <{{ page.contactEmail }}>.

Implementation guide: [{{ page.guidebook.linkText }}]({{ page.guidebook.url }})

</div>
</div>

</section>

</div>

<aside id="footnotes-aside" class="wb-fnote hidden" role="note">
<h3 id="fn">{{ site.Footnotes[ page.lang ] }}</h3>
<dl>
<dt>{{ site.Footnote[ page.lang ] }} 1</dt>
<dd id="fn1">
<p>Under the [Privacy Act](http://laws-lois.justice.gc.ca/eng/acts/P-21/index.html), personal information, as defined by, is <q cite="http://laws-lois.justice.gc.ca/eng/acts/P-21/page-1.html#h-3">"information about an identifiable individual that is recorded in any form."</q> For details, see section 3 of the act.</p>
<p class="fn-rtn"><a href="#fn1-rf"><span class="wb-inv">{{ site.ReturnToFootnote[ page.lang ] }} </span>1{% if page.lang == "en" %}<span class="wb-inv"> referrer</span>{% endif %}</a></p>
</dd>
</dl>
</aside>

</div>

</form>
</div>
