# TEST-EasyCLA
Easy-CLA is a bot developed by the Linux Foundation for tracking CLA signatures on open source projects. This tool will replace the legacy CLA-Assistant bot for projects that were formerly part of the JS Foundation, and will be available for any OpenJS Foundation project that would like to use a CLA.

## FAQs

### Do I have to use a CLA for my project?
No. Projects that would prefer to use a DCO will be directed to use [probot-dco](https://github.com/probot/dco). The foundation is aware of an issue with the DCO implementation and users of GitHub's GUI; we will have a developed work around for this issue soon. 

All OpenJS Foundations should use either a CLA, DCO, or signed commits as a matter of good IPR hygiene.

### What is the OpenJS Foundation CLA?
In plain terms, the OpenJS Foundation's CLA says that the contributor 1) is legally able to make the contributions, 2) agrees to contribute to OpenJS Foundation projects in accordance with the licenses in their respective repositories, and 3) understands that their contributions are public. Contributors are responsible for reviewing these licenses and ensuring their contributions are compatible. 

Signing the [OpenJS Foundation CLA](https://openjsf.org/about/the-openjs-foundation-cla/) for a contribution you make to one project also enjoins contributions you make to other OpenJS Foundation projects. 

### Who needs to sign the OpenJS Foundation CLA?
Any committer to OpenJS Foundation projects that use a CLA needs to sign, regardless of whether they submitted the PR.

Once you have signed it for one OpenJS Foundation project, you will not need to sign it again to contribute to another Foundation project using the CLA.

### How does Easy-CLA work?
You can test the user flow for Easy-CLA by submitting a PR to this repo. When a contributor submits a pull request, Easy-CLA checks to see if that contributor's GitHub account has agreed to the OpenJS Foundation CLA. If it has, the check passes and the PR can be merged.

If the contributor has not signed the OpenJS Foundation CLA, the bot directs them (and all parties with commits on the PR who have not signed the CLA) to authorize the Easy-CLA app to read their GitHub account data. After authorization, the contributor is taken to the Community Bridge Easy-CLA app. In the app, the contributor must choose whether they are contributing on behalf on an employer or as an individual.

#### Contributing as an Employee
If contributing on behalf of an employer, the contributor should select 'Corporate', select their employer from the list, and continue with the instructions. Corporate contributors' commitments are covered under an [Corporate Contributor License Agreement](https://openjsf.org/wp-content/uploads/sites/84/2020/01/OpenJS-Foundation-Corporate-CLA-2019-12-13.pdf). **If your employer is not listed,** follow the instructions to notify your corporate CLA Manager to create an account with the Linux Foundation and add your GitHub username to their list of permitted users. 

**If your employer is listed but you are not on the list of permitted users,** you will get a message directing you to check your GitHub settings and/or notify the company CLA Manager that you need to be added to the list of allowed users.  

#### Contributing as an Individual
If you are contributing on behalf of yourself - meaning that no other person or entity could make a claim on your contributions - select 'Individual' and follow the instructions to electronically sign the [Individual CLA](https://individual-cla.openjsf.org). This will present you with an Individual Contributor License Agreement via docusign, which you can download and save.

### Can I add bot accounts to an 'allowlist'?
Yes. If you use automation bots for CI and that sort of thing, the Foundation can exempt them from the Easy-CLA process.

### What if my employment status changes?

Your former company's CLA manager will need to remove you from their allowlist as part of your off-boarding from the company. Your next PR will trigger the Easy-CLA tool for signature, and you will need to sign again either as an Individual or as part of your new company.

### How do I add Easy-CLA to my project?

Email operations@openjsf.org or talk to Brian Warner. Easy-CLA can be added to every repo in your org or just a few (you may not want to add it to your admin repo, for example).

### How do I find out who my CLA Manager is?
_working on this_

### My project is moving from the old JS Foundation CLA to the Easy-CLA. What do I need to know?

* **Your contributors will need to re-sign the CLA.** The CLA Assistant tool bound contributions to the CLA of the former JS Foundation. They will need to re-sign as the legal entity has changed.
* **Provide a list of permitted bots in advance.** We will make sure these tools are not caught by the Easy-CLA tool.
* **If you have a lot of contributors, we can help jump start the process for contributions that will be covered under a Corporate CLA.** We can work with you and your maintainer team to make sure that your biggest recurring contributors are not unduly inconvenienced the next time they submit a PR.
* **It's a good idea to message this upcoming change in advance.** This will let your community know what changes to expect, why, and give them a chance to review the CLA or get their company to sign or update their Corporate CLA. 
* **This is the same tool used by 100s of Linux Foundation projects.** That means _a lot_ of companies have signed the Corporate CLA already, and a lot of your contributors (or would be contributors) are likely covered. 