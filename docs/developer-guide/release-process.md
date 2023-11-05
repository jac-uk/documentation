---
nav_order: 3
parent: Developer guide
---

# Deployment

## Versioning
We use an adaptation of the Semantic Versioning Specification **MAJOR.MINOR.PATCH** adapted to our needs


**MAJOR** revision (new UI, lots of new features, conceptual change, etc.) - we don't change this very often

**MINOR** revision (maybe a change to a search box, 1 feature added, collection of bug fixes) - basically every daily release we increment this number

**PATCH** - bugfix - Whenever we do a hotfix, we increment this number between daily releases


## Release Process

We use Github Actions with the existing Github UI and follow Github Flow model for organising our source code, releases and hotfixes.

![1](./images/release.png)

Benefits of the process:

* It is simple
* Early approval per feature
* Puts control in hands of whole team
* Can easily be refined

### Developer workflow

<a target="_blank" rel="noopener noreferrer" href="/jac-uk/documentation/blob/master/docs/developer-guide/images/release7.png"><img src="/jac-uk/documentation/raw/master/docs/developer-guide/images/release7.png" alt="2" height="50px"></a>

<a target="_blank" rel="noopener noreferrer" href="/jac-uk/documentation/blob/master/docs/developer-guide/images/release8.png"><img src="/jac-uk/documentation/raw/master/docs/developer-guide/images/release8.png" alt="3" height="50px"></a>

<a target="_blank" rel="noopener noreferrer" href="/jac-uk/documentation/blob/master/docs/developer-guide/images/release9.png"><img src="/jac-uk/documentation/raw/master/docs/developer-guide/images/release9.png" alt="4" height="50px"></a>

1. Developer takes their next ticket from top of the ‘Current and next sprint’ column moving it to ‘In progress’ or ‘Blocked’ if there is a problem.

2. When developer is ready, they create a new Pull Request and move ticket to ‘Ready for Review’. Their work is automatically deployed to a preview URL. The setting for the preview url is located at the end of the pull request description and can be set to `PREVIEW:OFF, PREVIEW:DEVELOP or PREVIEW:STAGING`.

3. We now need exactly one approval each from in-house developers, both contractors, product owner and User Testing Group.

4. If all developers approve changes before PO & UTG, then the ticket can be moved to ‘Code Approved’.

5. When approved and merged the change is automatically deployed to Staging.

6. Whenever changes are approved and merged the next draft release is updated.

7. When a draft release is published the changes are automatically deployed to Production.

8. To roll back or forwards to a specific version we use a manual Action called ‘Deploy to Production’.

![5](./images/release5.png)

![6](./images/release6.png)

After the release post these release notes to Slack channel **#digital-team** using the following format:

> @channel version **[VERSION]** has been released to **[APP]** production
> 2 issues / 16.5 sp
>
> https://**[APP]**.judicialappointments.digital/
>
> *#123 Add cancel button to sign up page
>
> *#124 Add log out button to header

Finally add the same message to the respective apply/admin section of the release notes email.

---
