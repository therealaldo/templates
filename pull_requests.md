# Pull Requests Template

Below is the template for how to open and submit PRs to Ultrasound. Small pull requests are much easier to review and more likely to get merged. Make sure the PR does only one thing, otherwise please split it.

Please make sure the following is completed when submitting a pull request:

1. Fork the repository and create your branch from `master`.
1. Describe your test plan in your pull request description. Make sure to test your changes!
1. If you haven't already, sign the CLA before submitting your pull request.

## Format

Our goal is to have descriptive, relevant information that pertains to the pull request attached, whether that be by adding screenshots where appropriate or even having additional information based on the type of change it may be. The format for PRs is as follows:

* **Description**
* **Motivation &amp; Context**
* **How Has This Been Tested?**
* **Screenshots (if appropriate)**
* **Types of Changes**
* **Checklist**

---

### Description

Provide a description summarizing what your pull request is for.

> Adding the ability to transform text within the app. My test plan involves having added a test-case to the RNTester app within the `<Text>` component area. I then manually verified that the rendered content met my expectation.

#### Test Plan

A good test plan has the exact commands you ran and their output. Also provide screenshots or videos if your pull request changes the UI.

* If you've added code that should be tested, add tests!
* If you've changed APIs, update the documentation.

See [What is a Test Plan?](https://medium.com/@martinkonicek/what-is-a-test-plan-8bfc840ec171#.y9lcuqqi9) to learn more.

---

### Motivation and Context

Let us know what your motivation and context are for opening your pull request.

> The basic desire is to have a declarative mechanism to transform text context to uppercase or lowercase or titlecase ("capitalized").

---

### How Has This Been Tested?

Let us know how your pull request has been tested. If tests need to be written for your pull request, a great suggestion would be to write your tests yourself for a better chance of the request being accepted.

>

---

### Screenshots (if appropriate)

Provide screenshots of the changes made in your pull request if it would help in understanding the change.

> Here is the markup that exercises my enchancement:
>
> ```text
> <View>
>   <Text style={{ textTransform: 'uppercase'}}>
>     This text should be uppercased.
>   </Text>
>   <Text style={{ textTransform: 'lowercase'}}>
>     This TEXT SHOULD be lowercased.
>   </Text>
>   <Text style={{ textTransform: 'capitalize'}}>
>     This text should be CAPITALIZED.
>   </Text>
>   <Text style={{ textTransform: 'capitalize'}}>
>     Mixed:{' '}
>     <Text style={{ textTransform: 'uppercase'}}>
>       uppercase{' '}
>     </Text>
>     <Text style={{ textTransform: 'lowercase'}}>
>       LoWeRcAsE{' '}
>     </Text>
>     <Text style={{ textTransform: 'capitalize'}}>
>       capitalize each word
>     </Text>
>   </Text>
> </View>
> ```
>
> And here is a screenshot of the result
>
> ![text transform example](https://user-images.githubusercontent.com/575821/37433772-7abe7fa0-279a-11e8-9ec9-fb3aa1952dad.png?raw=true)

---

### Types of Changes

Let us know the types of changes you made in your pull request. The types of changes you can make are:

* **Bug fix** (non-breaking change which fixes an issue)
* **New feature** (non-breaking change which adds functionality)
* **Breaking change** (fix or feature that would cause existing functionality to not work as expected)

> * [x] Bug fix
> * [x] New feature

#### Bug Fixes

When adding a new big fix change, add the issues your pull request fixes.

> Fixes: #18451 \
> Fixes: #18663

#### Breaking Changes

When adding a new breaking change, add the additional information below to your pull request.

* **Who does this affect?**
* **How to migrate**
* **Why are you making this breaking change?**
* **Severity** (number of people affected x effort)

> **Who does this affect?** \
> This affects any user using any version before 1.0.0
>
> **How to migrate** \
> Update to the newest version of Ultrasound
>
> **Why are you making this breaking change?** \
> Providing the ability to scroll smoother on list headers
>
> **Severity** \
> Although many people are affected by this breaking change, all they would need to do is update to the newest version of the app.

---

### Checklist

Fill out the checklist with all of the options selected that apply to your pull request.

> * [x] My code follows the code style of this project
> * [x] My change requires tests to be written
> * [x] I have written the tests necessary for my code
> * [x] My change requires a change to the documentation
> * [x] I have updated the documentation accordingly
