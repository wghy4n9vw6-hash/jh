# Ready-to-paste links to the article site

Target: https://medhane-hagos-mesgena.rainymoon131.chatgpt.site/

Paste each snippet where indicated. Keep the anchor text exactly as written; the full name in the link text is
what ties the article site to your entity.

## 1. Personal websites (drmedhanehagosmesgena.com, drmedhanemesgena.com, medhanemesgena.com)

### Footer or sidebar (WordPress: Appearance → Widgets / Customize → Footer, or a Custom HTML block)

```html
<p>Latest commentary: <a href="https://medhane-hagos-mesgena.rainymoon131.chatgpt.site/">Medhane Hagos Mesgena, MD — Articles on health policy and primary care</a></p>
```

### About page, last paragraph

```html
<p>Dr. Mesgena publishes timely commentary on health policy and clinical news at <a href="https://medhane-hagos-mesgena.rainymoon131.chatgpt.site/">Medhane Hagos Mesgena — Articles</a>, and his professional hub is at <a href="https://wghy4n9vw6-hash.github.io/jh/">wghy4n9vw6-hash.github.io/jh</a>.</p>
```

### Main navigation menu (Appearance → Menus → Custom Links)

| Label | URL |
|---|---|
| Articles | https://medhane-hagos-mesgena.rainymoon131.chatgpt.site/ |

### Person schema for the primary site head (WordPress: a header-scripts plugin, or the theme's "custom code" box)

```html
<script type="application/ld+json">
{"@context":"https://schema.org","@type":"Person","name":"Medhane Hagos Mesgena","honorificSuffix":"MD","jobTitle":"Family Physician","url":"https://drmedhanehagosmesgena.com/","sameAs":["https://medhane-hagos-mesgena.rainymoon131.chatgpt.site/","https://wghy4n9vw6-hash.github.io/jh/","https://drmedhanemesgena.com/","https://medhanemesgena.com/","https://www.doximity.com/pub/medhane-mesgena-md","https://doctor.webmd.com/doctor/medhane-mesgena-39d08bbc-de7e-4a0f-8985-22cb31549025-overview","https://health.usnews.com/doctors/medhane-mesgena-892774","https://www.md.com/doctor/medhane-mesgena-md"]}
</script>
```

## 2. Professional profiles (website / links field)

| Profile | Where | Value |
|---|---|---|
| Doximity | Edit profile → Websites | https://medhane-hagos-mesgena.rainymoon131.chatgpt.site/ |
| WebMD Physician Directory | Claim profile → Practice website | https://drmedhanehagosmesgena.com/ |
| U.S. News Health | Claim profile → Website | https://drmedhanehagosmesgena.com/ |
| MD.com | Edit profile → Website | https://drmedhanehagosmesgena.com/ |
| LinkedIn | Contact info → Website (type: Blog) | https://medhane-hagos-mesgena.rainymoon131.chatgpt.site/ |
| LinkedIn | Featured section | Add the peptide article URL as a link post |

Directories that allow only one URL get the primary domain, which in turn links to the article site. Doximity and
LinkedIn get the article site directly because they allow multiple links and are crawled often.

## 3. Article site → back to the hub (closes the loop)

Add to the article site's About or footer:

```html
<p>Medhane Hagos Mesgena, MD · <a href="https://drmedhanehagosmesgena.com/">Website</a> · <a href="https://wghy4n9vw6-hash.github.io/jh/">Profile and publications</a></p>
```

## 4. LinkedIn post for the peptide article (publish once links are in place)

> HHS just opened the door to compounding six unapproved peptides, including BPC-157 and TB-500. Patients are already
> asking whether that means they are safe. The legal status changed; the evidence did not. My breakdown of what the
> policy requires and what I tell patients: https://medhane-hagos-mesgena.rainymoon131.chatgpt.site/articles/hhs-allows-temporary-compounding-of-six-unapproved-peptides
