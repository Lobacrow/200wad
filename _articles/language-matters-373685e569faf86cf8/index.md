---
title: "Language matters"
created_at: 2020-02-27T00:41:19.000Z
published_at: 2020-02-27T00:52:46.000Z
---
It's time for a peek behind the curtain in my day job. I currently manage a configuration team responsible for maintaining a health insurance claims processing system. Someone submitted a ticket today for a claim that's triggering an edit.

The claim is for an exchange benefit plan (Obamacare). These health plans follow the US Preventive Task Force recommendations for preventive services. The service in question is a fluoride varnish for primary teeth to help prevent cavities.

Here is the language in question:

*   "The recommendation applies to children from birth through age 5 years."
*   "The USPSTF concludes with moderate certainty that there is a moderate net benefit of preventing future dental caries with fluoride varnish application in all children starting at the age of eruption of primary teeth to age 5 years."
*   "This recommendation applies to children age 5 years and younger."

How would you interpret and build this requirement to restrict the age for this benefit? The way our system is built, we have a maximum age on the benefit set at 59 months (4 years 11 months). We have a claim for a child who is 5 years and 2 months old, and that's the claim triggering an edit because the age restriction failed. 

I think the age restriction in the system is not consistent with the requirement. I interpret "age through 5 years" and "age 5 years and younger" as still applying to a 5 yr old. And you are 5 years old until you are 6 years old, technically speaking. It's not my call. My job is to build the requirements approved by the business. I'm waiting for a response.

Language matters especially when you try to interpret gray requirements into black and white programming for a computer system.
