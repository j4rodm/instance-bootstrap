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

# SN Security Universe: hybrid test

## D. Overview (static, clickable)

```mermaid
flowchart LR
    ROOT([SN Security Universe]) --> SEC[Security Operations]
    ROOT --> VR[Vulnerability Response]
    ROOT --> IRM[Integrated Risk Management]
    click SEC "https://www.servicenow.com/products/security-operations.html" _blank
    click VR "https://www.servicenow.com/products/vulnerability-response.html" _blank
    click IRM "https://www.servicenow.com/products/integrated-risk-management.html" _blank
```

## E. Mindmap (static)

```mermaid
mindmap
  root((SN Security Universe))
    Security Operations
      SecOps overview
      Podcast: Cyberthreat
      Docs
    Vulnerability Response
      VR overview
      Store listing
    Integrated Risk Management
      IRM overview
      Community guide
```

## F. Expandable links (click the arrows)

<details>
<summary><b>Security Operations</b></summary>

- Overview: [SecOps product page](https://www.servicenow.com/products/security-operations.html)
- Podcast: [Cyberthreat: Real Answers to Real Problems](https://podcasts.apple.com/podcast/id1439624860)
- Docs: [Product Documentation](https://docs.servicenow.com)

</details>

<details>
<summary><b>Vulnerability Response</b></summary>

- Overview: [VR product page](https://www.servicenow.com/products/vulnerability-response.html)
- Store: [VR on the Store](https://store.servicenow.com/store/app/21d8a32e1be06a50a85b16db234bcb7e)

</details>

<details>
<summary><b>Integrated Risk Management</b></summary>

- Overview: [IRM product page](https://www.servicenow.com/products/integrated-risk-management.html)
- Community: [Risk adoption guide](https://www.servicenow.com/community/grc-articles/welcome-to-servicenow-risk-get-started-on-your-product-adoption/ta-p/3038531)

</details>

## G. Mindmap link tests

```mermaid
mindmap
  root((SN Security Universe))
    Security Operations
      <a href="https://www.servicenow.com/products/security-operations.html" target="_blank">HTML anchor</a>
      ["[Markdown link](https://www.servicenow.com/products/security-operations.html)"]
      Plain text for comparison
```

## H. Link color tests

```mermaid
%%{init: {'theme':'base','themeVariables':{'primaryColor':'#e8f4f8','primaryTextColor':'#1a1a1a','lineColor':'#2a6f8f'}}}%%
mindmap
  root((SN Security Universe))
    Security Operations
      <a href="https://www.servicenow.com/products/security-operations.html" style="color:#d9480f">1 anchor style</a>
      <a href="https://www.servicenow.com/products/security-operations.html"><span style="color:#2b8a3e">2 inner span</span></a>
      <a href="https://www.servicenow.com/products/security-operations.html"><font color="#862e9c">3 inner font</font></a>
      Plain text for comparison
```
## I. Shared end node

```mermaid
flowchart LR
    ROOT([SN Security Universe]) --> SEC[Security Operations]
    ROOT --> IRM[Integrated Risk Management]
    SEC --> POD["<a href='https://podcasts.apple.com/podcast/id1439624860' style='color:#d9480f'>Podcast: Cyberthreat</a>"]
    IRM --> POD
    SEC --> SECDOC["<a href='https://www.servicenow.com/products/security-operations.html' style='color:#2b8a3e'>SecOps page</a>"]
    IRM --> IRMDOC["<a href='https://www.servicenow.com/products/integrated-risk-management.html' style='color:#2b8a3e'>IRM page</a>"]
```
## J. Flowchart link tests

```mermaid
flowchart LR
    ROOT([SN Security Universe]) --> A["<a href='https://www.servicenow.com/products/security-operations.html'><span style='color:#d9480f'>1 inner span</span></a>"]
    ROOT --> B["<a href='https://www.servicenow.com/products/security-operations.html'><font color='#2b8a3e'>2 inner font</font></a>"]
    ROOT --> C["<a href='https://www.servicenow.com/products/security-operations.html' target='_top'>3 target _top</a>"]
    ROOT --> D["<a href='https://www.servicenow.com/products/security-operations.html' target='_blank' rel='noopener'>4 target _blank</a>"]
    style A fill:#fff4e6,stroke:#d9480f
    style B fill:#ebfbee,stroke:#2b8a3e
```
## K. Cluttered map

```mermaid
flowchart LR
    ROOT([SN Security Universe])

    ROOT --> SEC[Security Operations]
    ROOT --> VULN[Exposure and Vulnerability]
    ROOT --> GRC[Risk and Compliance]

    SEC --> SIR[Security Incident Response]
    SEC --> TI[Threat Intelligence]
    VULN --> VR[Vulnerability Response]
    VULN --> CC[Configuration Compliance]
    GRC --> IRM[Integrated Risk Management]
    GRC --> TPR[Third-Party Risk]

    SIR --> OVSEC["<a href='https://www.servicenow.com/products/security-operations.html'><font color='#1c7ed6'>SecOps overview</font></a>"]
    VR --> OVVR["<a href='https://www.servicenow.com/products/vulnerability-response.html'><font color='#1c7ed6'>VR overview</font></a>"]
    IRM --> OVIRM["<a href='https://www.servicenow.com/products/integrated-risk-management.html'><font color='#1c7ed6'>IRM overview</font></a>"]

    SIR --> POD["<a href='https://podcasts.apple.com/podcast/id1439624860'><font color='#d9480f'>Podcast: Cyberthreat</font></a>"]
    TI --> POD
    IRM --> POD

    SIR --> DOCS["<a href='https://docs.servicenow.com'><font color='#2b8a3e'>Product Docs</font></a>"]
    VR --> DOCS
    CC --> DOCS
    IRM --> DOCS
    TPR --> DOCS

    VR --> STORE["<a href='https://store.servicenow.com/store/app/21d8a32e1be06a50a85b16db234bcb7e'><font color='#862e9c'>VR on the Store</font></a>"]
    CC --> STORE

    TI --> BLOG["<a href='https://www.servicenow.com/blogs.html'><font color='#e67700'>ServiceNow Blogs</font></a>"]
    TPR --> BLOG
    SIR --> BLOG

    GRC --> COMM["<a href='https://www.servicenow.com/community/grc-articles/welcome-to-servicenow-risk-get-started-on-your-product-adoption/ta-p/3038531'><font color='#0b7285'>Community: Risk guide</font></a>"]
    TPR --> COMM

    classDef area fill:#e7f5ff,stroke:#1c7ed6
    classDef sub fill:#f3f0ff,stroke:#7048e8
    classDef leaf fill:#fff9db,stroke:#f08c00
    class SEC,VULN,GRC area
    class SIR,TI,VR,CC,IRM,TPR sub
    class OVSEC,OVVR,OVIRM,POD,DOCS,STORE,BLOG,COMM leaf
```
