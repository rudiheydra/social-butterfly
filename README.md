# Lesson 10

Live Demo: [https://socialbutterfly.vercel.app/](https://socialbutterfly.vercel.app/)
<- Back to [previous lesson](https://github.com/mongodb-developer/social-app-demo/tree/9-lesson)

---

## Goal

The goal of this lesson is to deploy our completed project to Vercel.

> Be sure to switch to the `10-lesson` branch in your local environment.

- ~15 minutes of slides explaining Jamstack, serverless, and how the MongoDB Atlas Data API fits into these.
- Hands-on lesson resulting in you building a fully functional, deployed application.

## Task 1: Create a Vercel Account

If you don't already have a [Vercel account](https://vercel.com/signup), create one.

## Task 2: Create a Vercel Project

- Familiarity with JavaScript
- Accounts (All Free):
  - [MongoDB Atlas](https://www.mongodb.com/cloud/atlas/register2)
  - [GitHub](https://github.com/signup)
  - [Vercel](https://vercel.com/signup)
  - [Auth0](https://auth0.com/signup)
- Git and GitHub knowledge (fork, clone, branch, commit, etc.)
- Node.js installed on your computer (14.x / 16.x)
- Code Editor (VS Code recommended)

1. From the Vercel dashboard, create a new project.
1. Choose **Continue with GitHub**.
1. Find the **social-app-demo** repository in the list and choose **Import**.
1. Select **Next.js** as the framework.
1. Under **Environment Variables**, add all of your environment variables from your [`.env.local`](./.env.local) file.
1. Click **Deploy**.
   - This initail deploy will not really do anything since the `main` branch does not contain our final code.
1. Go back to the main dashboard and select your new project.
   - Take note of your custom domain. (Example: `https://socialbutterfly.vercel.app`)
1. From the **Settings** tab, click **Git**.
1. Change the **Production Branch** to `10-lesson` and save.
1. Navigate to the **Environment Variables** tab.
1. Change `AUTH0_BASE_URL` to your custom Vercel domain noted earlier.
1. To redeploy, you'll need to make a new commit to the `10-lesson` branch. You can simply open the `README.md` file, add a space somewhere, and make a new commit.

## Task 3: Update Auth0 settings

## Slides

- [Workshop Slides](https://docs.google.com/presentation/d/1UuJl2kyuUfkDJah6WqSGa59ZTKtLK2SN-mMgUtAGqR0/edit?usp=sharing)

## Hands-on lesson

This repo is broken up into several branches. Each branch contains a set of lesson and builds upon the previous lesson.

Throughout the workshop, you'll be working on the following lessons:

1. [Lesson 1 - Fork & Clone Repo](https://github.com/mongodb-developer/social-app-demo/tree/1-lesson)
2. [Lesson 2 - Create Cluster & Enable Data API](https://github.com/mongodb-developer/social-app-demo/tree/2-lesson)
3. [Lesson 3 - Load Sample Data](https://github.com/mongodb-developer/social-app-demo/tree/3-lesson)
4. [Lesson 4 - Test Data API Endpoint](https://github.com/mongodb-developer/social-app-demo/tree/4-lesson)
5. [Lesson 5 - Setup CRUD Endpoints](https://github.com/mongodb-developer/social-app-demo/tree/5-lesson)
6. [Lesson 6 - Overview of Data API App](https://github.com/mongodb-developer/social-app-demo/tree/6-lesson)
7. [Lesson 7 - Setup Custom User Authentication](https://github.com/mongodb-developer/social-app-demo/tree/7-lesson)
8. [Lesson 8 - Add "Like" Functionality](https://github.com/mongodb-developer/social-app-demo/tree/8-lesson)
9. [Lesson 9 - Create a Search Index and Implement Search Functionality](https://github.com/mongodb-developer/social-app-demo/tree/9-lesson)
10. [Lesson 10 - Deploy to Vercel!](https://github.com/mongodb-developer/social-app-demo/tree/10-lesson)
11. In your Auth0 application, update the following fields under **Settings**:

- Allowed Callback URLs: `http://localhost:3000/api/auth/callback, https://*.vercel.app/api/auth/callback`
- Allowed Logout URLS: `http://localhost:3000, https://*.vercel.app, http://*.vercel.app`
- Allowed Web Origins: `https://*.vercel.app`

---

Let's get started with the [first lesson](https://github.com/mongodb-developer/social-app-demo/tree/1-lesson) ->
Great job! Your application is now deployed and you can open it from the **Overview** tab in Vercel or by navigating to your custom Vercel domain.

## Bonus: Team Collaboration

Team up with someone and browse to each other's deployed applications. Leave some flutters to let them know it's working.
