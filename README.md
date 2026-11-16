# SN Security Universe: render test

## A. Nested details

<details>
<summary><b>Security Operations</b></summary>

- Overview: [SecOps product page](https://www.servicenow.com/products/security-operations.html)
- Podcast: [Cyberthreat: Real Answers to Real Problems](https://podcasts.apple.com/podcast/id1439624860)
- Blog: [ServiceNow Blogs](https://www.servicenow.com/blogs.html)
- Docs: [Product Documentation](https://docs.servicenow.com)
- Video: [ServiceNow on YouTube](https://www.youtube.com/@servicenow)

<details>
<summary><b>Vulnerability Response</b></summary>

- Overview: [VR product page](https://www.servicenow.com/products/vulnerability-response.html)
- Store: [VR on the Store](https://store.servicenow.com/store/app/21d8a32e1be06a50a85b16db234bcb7e)

</details>
</details>

<details>
<summary><b>Integrated Risk Management</b></summary>

- Overview: [IRM product page](https://www.servicenow.com/products/integrated-risk-management.html)
- Community: [Risk adoption guide](https://www.servicenow.com/community/grc-articles/welcome-to-servicenow-risk-get-started-on-your-product-adoption/ta-p/3038531)

</details>

## B. Mermaid with click directives

```mermaid
flowchart LR
    ROOT([SN Security Universe]) --> SEC[Security Operations]
    ROOT --> IRM[Integrated Risk Management]
    SEC --> SEC1[SecOps product page]
    IRM --> IRM1[IRM product page]
    click SEC1 "https://www.servicenow.com/products/security-operations.html" _blank
    click IRM1 "https://www.servicenow.com/products/integrated-risk-management.html" _blank
```

## C. Mermaid with Markdown links in labels

```mermaid
flowchart LR
    ROOT([SN Security Universe]) --> SEC[Security Operations]
    ROOT --> IRM[Integrated Risk Management]
    SEC --> SEC1["[SecOps product page](https://www.servicenow.com/products/security-operations.html)"]
    IRM --> IRM1["[IRM product page](https://www.servicenow.com/products/integrated-risk-management.html)"]
```
