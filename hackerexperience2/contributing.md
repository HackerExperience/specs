# Introduction

As a whole, we seek *universal contribution*, i.e. a place where anyone can share their opinion regarding a specific part of the project. In order to achieve universal contribution, we need a framework that is

 - **Simple**, 
 - **Reactive**, so discussions get fast feedback, often;
 - **Clear**, so contributing guidelines can easily be followed;
 

This framework prevents some common problems with OSS. Mainly, we don't want the contributor to feel:

- **intimidated**:
    - "There is nothing useful I can add to these discussions";
    - "I don't understand their commit review process"
    - "So many rules. They won't accept my contributions due to minor errors".
- **frustrated**:
    - "I've submitted this patch but I haven't received any responses yet";
    - "My questions don't get answered"


We've found [Phabricator](http://phabricator.org) to be the best OSS tool that could allow us meet these requirements. However, Phabricator's interface and usability might take some time to get used to.

# Getting started 

- Visit our [development center](https://dev.hackerexperience.com) and create an account (or log in with any social network). Meet Phabricator!

    - First of all, **don't panic**.
    - Phabricator's interface *is* hard-to-use. It might take a while, but you'll get used to it. Don't worry.
    
    
- Now, a quick explanation on how Phabricator works.  
    - Phabricator is an all-in-one (AIO) place to develop, discuss and review HE2. All you need is there.
    - Phabricator is made of many different applications, each with its own purpose. Some of them are:
        - **Maniphest**: the place where you can create a **task**, or bug report, to be analysed and discussed.
        - **Differential** is the code review utility, where developers will discuss and accept/deny changes to HE2 code.
        - **Diffusion**, where all repositories related to, or owned by HE2 are. You can browse their code there.
        - **Conpherence** is a chat utility, where you can join private or public groups and talk about anything. Keep in mind that Conpherence is not the place for important discussions, they belong to Maniphest. It's a nice place to introduce yourself and get help from other contributors.
        - **Projects** allow people to be grouped by interests or content. It works like tags. A question about game-design will belong to the "Game Design" tag (and any other, if relevant). Then, you can find all tasks related to "Game Design".


- Now we will guide you according to how you can/want to help.
- Don't worry if you make a mistake, or ask on the wrong part of the site. No one will *bit* you :)


# I want to...

## 1 - Ask something

Usually, you'll want to ask questions on [Ponder](https://dev.hackerexperience.com/ponder/), a Q&A phabricator application pretty much like StackOverflow or Quora. In some rare cases, however, a question needs proper discussion, so creating a task is the way to go. Below is a simple procedure to follow.

- If it's something that needs proper discussion, review or approval, create a task [(see below)]().
- If it's something personal, go to Conpherence.
    - There, join the room most suitable for your question (use "General" if none fit).
    - Ask :)
- Go to [Ponder](https://dev.hackerexperience.com/ponder/).
- On the upper right corner, click [Ask Question](https://dev.hackerexperience.com/ponder/question/create/).
    - Enter your question on "Question Details".
    - You can ignore "Answer Details". This is usually for self-answered questions.
    - (optional) Add projects related to the question. Start typing something related and see if Phabricator finds anything.
    - Click "Send" & wait for your answer.

## 2 - Create a task, discussion, report a bug or request a feature:

First, ask yourself: is what your are going to ask/report something that needs discussion, review and approval? If it is a simple or straightforward question, see [Ask Something]() above. Don't worry if you are unsure.

Usually, bug reporting and requesting/suggesting a feature requires proper discussion, review and approval.

- Go to [Maniphest](https://dev.hackerexperience.com/maniphest/)
- On the upper right corner, click *Create Task*. Select the type of task (Feature Request, Report a bug, ...). If you can't find a correct type, select [Custom Task](https://dev.hackerexperience.com/maniphest/task/edit/form/2/).
- Enter your question.
    - On *Title*, enter a meaningful and descriptive title.
    - On *Description*, enter your report/discussion. Be the most descriptive and detailed you can be.
    - (optional) Add projects related to the task. Start typing something related and see if Phabricator finds anything.
    - You can ignore any other fields.
    - Click on *Create New task* & wait for your answer.

## 3 - Help with stuff I'm good at (includes non-tech)

That's great! At Phabricator, we tag all Tasks with corresponding projects, exactly to allow you to find very specific stuff.

Want to find tasks related to Linux? Or Docker? Or Design/UI? Maybe Elm? No problem!

- Go to [Active Projects](https://dev.hackerexperience.com/project/query/active/)
    - See which ones interest you.
    - Subscribe to them to receive in-phabricator updates.
    - See open tasks on workboards for tasks in need of help.
        - If the project does not have a workboard enabled, use the [Task Search](https://dev.hackerexperience.com/maniphest/query/advanced/) and add the project tag.

Non-tech projects include Translation, GameDesign, FeatureRequest, SocialMedia, Marketing, Legal.

## 4 - Clone a repository

Cloning a repository is easy. First of all, you need to set up your cloning credentials. It's very straightforward.

If you have SSH Keys set up, using the Clone (SSH) option is faster. Otherwise, you should use Clone (HTTP).


- Make sure you have already added your cloning credentials for SSH or HTTPS. It's simple!
- Go to the repository main page. [Diffusion](https://dev.hackerexperience.com/diffusion) lists all repositories.
- Copy the Clone URL of SSH or HTTPS. If you have both credentials set up, SSH is better.
- On your terminal, type `git clone <url>` and that's it!

## 5 - Submit a change

- First, make sure there is a task related to your change. If not, create one (see 2), describing your changes and why you did them.
- TODO: requires arc

## 6 - Create a public project

- Please create a task (see 1) asking about the project, its name and purpose. If approved, we will create the project and give you moderator access to the project.

## I don't know
- See below.

# How can I help the project?

In many ways, even if you are not a developer. Let's go:

## Programmers

- Fix reported bugs (See Tasks with project Bugs).
- Fix TODOs (See Tasks with project [TODO](https://dev.hackerexperience.com/tag/todo/))
- Develop new features (See project [Features-Backlog](https://dev.hackerexperience.com/tag/features-backlog/))
- Others (See pynosso, Helix, Pheeb, Curupira, core)
- Follow/discuss/fix tasks of your preferred languages/applications [(see 3)]().

## System administrators

- Join discussions on tasks about [Infrastructure](https://dev.hackerexperience.com/tag/infra/), [Linux](https://dev.hackerexperience.com/tag/linux/), [Docker](https://dev.hackerexperience.com/tag/docker/) and many more. Weigh in!

## Network administrators

## Security Engineers

- Help us on tasks tagged with [Security](https://dev.hackerexperience.com/tag/security/) and [Critical](https://dev.hackerexperience.com/tag/critical).
- Review some critical packages (TODO: link).

## Game Designers

- Create the game mechanics with us! See discussions under [Game Design](https://dev.hackerexperience.com/tag/game_design/) and kindly share your opinion.
- Add feature requests.

## Translators

- Help us translate the game to your favorite language.

## English Speakers

Our in-house team is based in Brazil and we are not native English speakers. This means that many of our texts, documents, articles, tasks have grammar errors and typos, or are hard to understand.

- Through our Documentation website, we have *Improve this page* on each document.
  - Help us make those documents easier to understand.
  - Fix grammatical errors or misspellings.
- Check the [Grammatical Errors](https://dev.hackerexperience.com/tag/grammatical_errors/) project.

## Others / Non-technical / Everyone / Anyone
Stuff that doesn't require specific knowledge (so **anyone** can help).

- Translate the game.
- Suggest new features.
- Spread the word
- Donate / pre-order