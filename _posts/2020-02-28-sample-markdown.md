---
layout: post
title: Cloud Computing in Public Health
subtitle: It's about damn time 
author: Scarlett Thomas
---

{: .box-success}
Imagine this: you're hired to help tackle the day-to-day public health response during one of the most impactful pandemics of your lifetime.  You put on your epi hat, ready to use your training to track and diminish disease spread.  You open your laptop and are given access to all of the tools available.  Cue dumbfounded blinking.  A google sheets spreadsheet whose data has been manually input by other epidemiologists combing through lab reports?  You've gotta be kidding me.  

These were my thoughts 4.5 years ago when I was hired as an analytical epidemiologist to help support the COVID-19 response in healthcare facilities.  The realities of how siloed and technologically behind the state department of health was set in quickly when I was asked to create dashboards and situation reports to communicate the impacts of the spread and our current containment efforts.  

**Here is some bold text**
Cloud computing has revolutionized public health surveillance and decision-making, particularly in tracking infectious diseases across healthcare settings. The paper by Katapally and Ibrahim on digital health dashboards serves as an excellent starting point to explore this topic further.

## Cloud-Based Infrastructure for Public Health Surveillance

The authors of the study utilized Amazon Web Services (AWS) to create a secure and scalable infrastructure for their digital health dashboard[1]. This approach demonstrates the power of cloud computing in public health:

1. Virtual Private Clouds (VPCs): Two VPCs hosted on AWS provided secure environments for data storage and communication between the database, Progressive Web Application (PWA), and digital health dashboard[1].

2. Scalability: Amazon Elastic Compute Cloud (EC2) servers offer the flexibility to scale resources up or down based on demand, crucial for handling sudden outbreaks or increased data loads[1].

3. Secure Data Management: Amazon Relational Database servers ensure secure storage and management of sensitive health data[1].

## Tracking Infectious Diseases Across Healthcare Settings

For tracking the movement of infectious diseases, particularly Multi-Drug Resistant Organisms (MDROs), across different healthcare settings, cloud computing offers several advantages:

### Real-Time Data Collection and Analysis

Cloud-based systems like the Hospital Automated Laboratory Reporting (HALR) system can provide early reporting of specified pathogens, allowing for early detection of outbreaks and trend analysis[5]. This real-time capability is crucial when patients move between different healthcare settings.

### Interoperability and Data Sharing

Cloud platforms facilitate seamless data sharing between different healthcare facilities. When a patient is transferred from an OR to recovery, and then to a nursing home, their infection status can be instantly updated and shared across all relevant systems[3].

### Advanced Analytics and Machine Learning

Cloud computing enables the use of advanced analytics and machine learning algorithms to predict the spread of MDROs based on patient movement patterns and facility characteristics[3].

## National Healthcare Safety Network (NHSN)

The CDC's National Healthcare Safety Network (NHSN) is a prime example of how cloud computing can be leveraged for nationwide infectious disease surveillance:

1. Secure, Internet-based surveillance system for submitting both patient and healthcare personnel safety data[2].

2. Standardized definitions and risk-adjusted infection rates allow for benchmarking across facilities[2].

3. Provides valuable data on the frequency and antimicrobial susceptibility of pathogens[2].

## Future Directions

The CDC's recent $189 million cloud computing project aims to modernize its IT infrastructure, develop advanced analytic capabilities, and ensure more effective cybersecurity[3]. This initiative will likely enhance the ability to track and respond to infectious diseases across various healthcare settings.

By leveraging cloud computing, public health officials can create a more interconnected, responsive, and effective system for tracking and controlling the spread of infectious diseases, including MDROs, as patients move through different healthcare settings. This approach not only improves patient safety but also contributes to more efficient and targeted infection control strategies.



## Here is a secondary heading

[This is a link to a different site](https://deanattali.com/) and [this is a link to a section inside this page](#local-urls).

Here's a table:

| Number | Next number | Previous number |
| :------ |:--- | :--- |
| Five | Six | Four |
| Ten | Eleven | Nine |
| Seven | Eight | Six |
| Two | Three | One |

You can use [MathJax](https://www.mathjax.org/) to write LaTeX expressions. For example:
When \\(a \ne 0\\), there are two solutions to \\(ax^2 + bx + c = 0\\) and they are $$x = {-b \pm \sqrt{b^2-4ac} \over 2a}.$$

How about a yummy crepe?

![Crepe](https://beautifuljekyll.com/assets/img/crepe.jpg)

It can also be centered!

![Crepe](https://beautifuljekyll.com/assets/img/crepe.jpg){: .mx-auto.d-block :}

Here's a code chunk:

~~~
var foo = function(x) {
  return(x + 5);
}
foo(3)
~~~

And here is the same code with syntax highlighting:

```javascript
var foo = function(x) {
  return(x + 5);
}
foo(3)
```

And here is the same code yet again but with line numbers:

{% highlight javascript linenos %}
var foo = function(x) {
  return(x + 5);
}
foo(3)
{% endhighlight %}

## Boxes
You can add notification, warning and error boxes like this:

### Notification

{: .box-note}
**Note:** This is a notification box.

### Warning

{: .box-warning}
**Warning:** This is a warning box.

### Error

{: .box-error}
**Error:** This is an error box.

## Local URLs in project sites {#local-urls}

When hosting a *project site* on GitHub Pages (for example, `https://USERNAME.github.io/MyProject`), URLs that begin with `/` and refer to local files may not work correctly due to how the root URL (`/`) is interpreted by GitHub Pages. You can read more about it [in the FAQ](https://beautifuljekyll.com/faq/#links-in-project-page). To demonstrate the issue, the following local image will be broken **if your site is a project site:**

![Crepe](/assets/img/crepe.jpg)

If the above image is broken, then you'll need to follow the instructions [in the FAQ](https://beautifuljekyll.com/faq/#links-in-project-page). Here is proof that it can be fixed:

![Crepe]({{ '/assets/img/crepe.jpg' | relative_url }})
