Terms And Privacy
================

Terms of use and privacy policy abstracted out of the acme corporation website.

Usage
------
```yaml
# In your config.yaml
module:
  imports:
    - path: github.com/hugoinaction/TermsAndPrivacy
params:
  TermsAndPrivacy:
    company_name: <Your company>
    contact_email: <contact email for your company>
    website: <Website URL>
    contact_dpo_email: <Data Protection Officer Email>
    contact_dpo_phone: <Data Protection Officer Phone number>
```


Template
--------  
```
Exmaple
   <div class="title">
      <h2>
        {{ with .Param "TermsAndPrivacy.company_name" }}
          {{.}}&trade;
        {{ end }}
        {{with .Title}}
        {{. }}
      {{end}}
        
  </h2>
  </div>
```
