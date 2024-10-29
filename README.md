# Jekyll Job Market Site Setup and Configuration

Welcome to the guide for setting up your professional economics job market website. This template was adapted for NIU Graduate Students by [AdamBougher](https://github.com/adambougher) and [drklis](https://github.com/drklis/) based on the design used by [pwills.com](http://www.pwills.com), which is hosted on GitHub Pages and utilizes the elegant [Minimal Mistakes template](https://github.com/mmistakes/minimal-mistakes).

The site is built using Jekyll, a powerful static site generator, providing a clean and professional layout for showcasing your academic profile. This setup allows for easy customization while maintaining a polished appearance suitable for the economics job market. You may wish to complete the [Microsoft Learn tutorial](https://learn.microsoft.com/en-us/training/modules/create-host-web-sites-github-pages/) and associated [GitHub interactive exercise](https://github.com/skills/github-pages) in order to go over the basics prior to setting up your website with this template.

### Purpose of a Job Market Profile Website

In the competitive landscape of the economics PhD job market, having a professional online presence is crucial, regardless of your target (academia, government, industry/tech). A well-designed personal website serves multiple purposes:
1. It showcases your research, teaching experience, and professional background in one centralized location.
2. It provides easy access to your CV, job market paper, and other relevant documents for potential employers.
3. It can demonstrate your technical skills and attention to detail, qualities that are valued in the field of economics.
4. It offers a platform to share your academic interests, ongoing projects, and professional goals.

### Why This Template?

This template offers several advantages for students going on the job market:

- **Clean and Professional Design**: The Minimal Mistakes theme provides a simple, modern look that works well for academic profiles.
- **Cost-Effective**: Hosted on GitHub Pages, this solution is completely free, allowing you to allocate your resources elsewhere in your life/job search.
- **Customizable**: While maintaining a professional appearance, the template is flexible enough to reflect your individual academic identity.
- **Easy to Implement**: The following instructions are detailed and user-friendly, making it accessible even for those with limited web development experience while also improving your coding skills.

## Getting Started

In order to use this template, you will want to make sure you have a GitHub account. For more documentation on how to use a similar template with Git on your machine, please check out the [pwills.com repo](https://github.com/peterewills/peterewills.github.io) directly.

### Step 0: Sign up for GitHub

If you do not yet have a GitHub account, sign up for one. An easy guide to doing so is available [here](https://docs.github.com/en/get-started/start-your-journey/creating-an-account-on-github).
- Make sure to choose a professional sounding username! Stay away from silly words and numbers. Consider something simple and identifiable, such as JaneDoe, mkowal, or JSmithNIU. *You can change your username; please see instructions for doing so [here](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-user-account-settings/changing-your-github-username).*
- Use your university email address in making your account to be eligible for GitHub Education, which has numerous benefits. Follow [these instructions on applying to GitHub Education](https://docs.github.com/en/education/explore-the-benefits-of-teaching-and-learning-with-github-education/github-education-for-students/apply-to-github-education-as-a-student) as a student.

## Detailed Instructions

The instructions that follow will guide you step-by-step through the process of setting up your own professional economics job market website. Whether you're tech-savvy or new to web development, these detailed instructions will help you create a polished online presence to support your job market journey. *Let's get building!*

### Step 1: Clone this Repository

Steps 1-3 are preparatory steps to prepare your repo, content, and page setup. Step 4 will actually launch your page.

1. Click the green "Use this template" button.
2. In the dropdown menu, right-click "Create new repository" and open it in a new tab.
3. Name your repository professionally, e.g., "Jane-Doe-Profile" or "John-Smith-Academic".
4. You can leave description blank, or you can write a meaningful phrase like "My Jekyll job market profile".
5. Make sure the repository is set to "Public".
6. Click "Create repository".
7. Keep these instructions open in a separate tab. If you accidentally close the tab, the instructions will automatically be included in your new repo as the README.md file.

### Step 2: Upload Your Documents

1. In your new repository, navigate to the `assets/images` folder.
2. Click "Add file" > "Upload files".
3. Upload your professional headshot(s) and an image of your email address that is slightly warped.
    - Resize your headshot before uploading: Aim for a width of around 300-500 pixels. This ensures fast loading times without sacrificing image quality.
    - You may want two headshots -- one for the author profile in the sidebar and another for the landing page.
    - Create a warped email address[^1] image: Aim for a width of around 150-200 pixels.  
        - *Option 1 (Photoshop/Illustrator)*: Type your email address, then use the warp tool to slightly distort it.  
        - *Option 2 (AI-generated)*: Use an AI image generator with a prompt like "A slightly warped email address on a white background, black text, email: `youremail@example.com`".  
        - *Option 3 (Online tools)*: Use free online image editors like Canva or Pixlr to create and warp text.  
4. Navigate to the `assets/docs` folder.
5. Click "Add file" > "Upload files".
6. Upload your CV and job market paper in PDF format.

### Step 3: Update _config.yml

1. In your repository, find and click on the `_config.yml` file.
2. Click the pencil icon to edit the file.
3. Update the following fields:
   - Find `title:` in the code and change "Jekyll Profile" to your full name (e.g. "Jane Smith"). *Make sure you keep the quotation marks around your entry here and in the following details in this file!*
   - Find `name:` and replace "A Free Job Market Profile in Jekyll" with "Jekyll Website for [Your Full Name]" or "Profile for [Your Full Name]".
       - Note: the square brackets here and in the following steps indicate a blank to fill in. Remove the square brackets when you put in your information (e.g. "Jekyll Website for Jane Smith").
   - Update `email:` with your professional email address.
   - Update `url:` to "https://[yourgithubusername].github.io".
   - Update `baseurl:` to "/[your-repo-name]" (e.g., "/Jane-Doe-Profile") for the name of the repo you're working in with this website.
   - Change `repository:` to "[yourgithubusername]/[your-repo-name]".
   - Update the file name in the header image to your headshot (this image is *not* the banner image at the top of every page; rather, it is the image that shows up when you link the website in a program the generates a preview of the site)
     ```
     header:
       image: /assets/images/[your-image-filename.extension]
     ```
   - Scroll down to `# settings for author profile`. Under `author:`
     - Update `name:` with your full name in quotation marks.
     - Change `avatar:` to "/assets/images/[your-image-filename.extension]".
     - Update `bio:` with a brief professional description of yourself.
     - Update `github:` with your GitHub username (if applicable).
     - Update `linkedin:` with your LinkedIn profile name, the part that comes after \in\ on your LinkedIn profile url (e.g. anna-klis-1337a150). Delete the fake profile and leave this blank if you do not have a LinkedIn.
4. Click "Commit changes".  
    - You can choose either "Commit directly to the `master` branch" or "Create a **new branch** for this commit and start a pull request." If you work slowly, follow these instructions carefully, and do not touch other settings, you can have some confidence in committing directly to the master branch.

### Step 4: Set Up GitHub Pages

1. Go to your repository's "Settings" tab.
2. Click on "Pages" in the left sidebar.
3. Under "**Source**", leave the option "Deploy from a branch" in place. Below that, under "**Branch**" select the branch you want to deploy (usually "main" or "master").
4. Leave "/(root)" for the folder.
5. Click "Save".
6. Go back to your repo's "Code" tab. On the right-side, find "**About**" and click the setting gear wheel next to it.
7. Check the box next to "**Use your GitHub Pages website**" which should immediately update the Website field to your "https://[yourgithubusername].github.io/[your-repo-name]/".
8. Click "Save changes".
9. Wait a few minutes for your site to be published.
10. Right-click the link now for your profile and open it in a new tab.

Now, every time you click "Commit changes" and commit directly to the master branch, you should be able to see your updates happen on your profile. You will need to hit refresh, and you may need to wait for a moment, even up to a few minutes. 

Hopefully, by following this guide, we limit any issues with page build. However, if your changes are not showing up, make sure to look at your code page and scroll down to **Deployments**. If you see a 🟢 (green circle) with a checkmark, then github-pages has been successful. If you see a 🟠 (orange/yellow circle), it is still building and deploying. If you see a red ❌, you will need to troubleshoot the deployment. Search for answers online, in the GitHub forums/documentation, or consulting with an AI like Claude.

### Step 5: Update index.md

In this step, you are setting up the landing page for your profile. This page welcomes individuals to your site and gives a description of your background.

1. In your repository, find and open the `index.md` file.
2. Click the pencil icon to edit.
3. Update the image link with your GitHub username, the name of the repo you're working in, and the file name of your headshot:
   ```
   <img src="https://github.com/[yourgithubusername]/[your-repo-name]/blob/main/assets/images/[your-image-filename.extension]?raw=true" width="50%" hspace="20" align="right">
   ```
4. Update the biography text to reflect your professional story.
5. Commit the changes.

### Step 6: Update Your CV Link

In this step, you'll ensure that the link to your CV is correctly set up in the navigation menu of your website.

1. Navigate to the `_data` folder and open `navigation.yml`.
2. Click the pencil icon to edit.
3. Find the "Curriculum Vitae" entry under `main:`.
4. Update the `url:` to `/assets/docs/[your-cv-].pdf`.
5. Commit the changes.
6. Wait a few minutes for your site to be published, and then refresh your profile to see your changes.

### Step 7: Update Your Research

This step involves customizing the research section of your website to showcase your academic work.

1. In the `_portfolio` folder, open `index.md`.
2. Click the pencil icon to edit.
3. Update the research sections with your own work:
   - If you do not have any publications, you can remove the `<h2 id="publications">Publications</h2>` anchored header.
   - Update the "Working Papers" section with your current research.
4. For each paper, update the title, description, and the name of the document to the name of your PDF: `[Download File]({{ site.baseurl }}/assets/docs/[your-paper].pdf)`
5. Commit the changes.
6. If you removed the **Publications** section title, you will need to update the `_data/navigation.yml` file:  
   - Like in **Step 6**, go to the  `_data` folder and open `navigation.yml`.  
   - Click the pencil icon to edit.  
   - Scroll down to `portfolio:`, and under the `children:` section, delete the two lines that delineate the **Publications** section:
     ```
           - title: "Publications"
             url: /portfolio/#publications
     ```
   - Commit the changes.
7. Wait a few minutes for your site to be published, and then refresh your profile to see your changes.

### Step 8: Update Teaching, Links, and Contact Pages

In this step, you'll finish personalizing your site by updating the Teaching, Links and Contact sections of your website to reflect your academic experience and interests.

1. Navigate to the `_pages` folder.
2. Open `teaching.md` and click the pencil icon to edit.
3. Update the content with your teaching experience using Markdown[^2] language to format the sections.
4. Commit the changes.
5. Navigate back to the `_pages` folder.
6. Open `links.md` and click the pencil icon to edit.
7. Update with links relevant to your field and interests. Remember that, in Markdown, a link follows the following structure:  
   ```[The Text that Appears](url of your link)```
8. Commit the changes.
9. Navigate back to the `_pages` folder.
10. Open `contact.md` and click the pencil icon to edit.
11. Update your campus office from "Out on the Field" (ECON grad students are in DuSable 470), update your office hours, and update the  of your warped email
    ```![image of email]({{site.baseurl}}/assets/images/[your-email-filename.extension])```
13. Commit the changes.
14. Wait a few minutes for your site to be published, and then refresh your profile to see your changes.

### Final Steps

1. Review your site by going to `https://[yourgithubusername].github.io/[your-repo-name]`.
2. Check all pages and links to ensure everything is working correctly. *Double check you've removed all the disclaimers about the template website!*
3. If you notice any issues, you can make further edits directly on GitHub or clone the repository to your local machine for more extensive changes.

Remember, it may take a few minutes for changes to appear on your live site after committing them. If you don't see your changes, try clearing your browser cache or viewing the site in an incognito/private browsing window. 

## Advanced Style Issues

- If you want to remove any pages, make sure to update the `navigation.yml` file as in **Step 6**. Just deleting the .md file won't work and might break your site!
- If you want to personalize the banner with a different image (like a photo or custom Canva banner), make sure to resize your image to a width of 1280 px and then upload it to the `assets/images` folder as in **Step 2**. Go through all the pages[^3] and update niubanner.png to your file name (with extension) in the header info of each page:
  ```
  header:
    image: /assets/images/[your-filename.extension]
  ```
- If you change the banner image, you may want to change the color of links. You can do so by navigating to the `asset` folder, opening the `css` subfolder, and then clicking the `main.scss` file. Click the pencil icon to edit. You can update the hex code in the `$primary-color:` and `$link-color:` sections with your [chosen color](https://htmlcolorcodes.com/color-picker/).
- The white background and black color at the bottom have been selected as a clean, professional-looking template. While I do not recommend changin these, if you really want something different, you configure the *skin* of the Minimal Mistakes theme. Read more about how to do so and browse the color skins [here](https://mmistakes.github.io/minimal-mistakes/docs/configuration/).
- Want a cleaner URL? You can purchase a domain of your name (or a version of it) using a service like [IONOS](https://www.ionos.com/domains/com-domain) or [GoDaddy](https://www.godaddy.com/). Domains are relatively inexpensive, especially compared to website building and hosting. You can then set up your GitHub profile to publish to your custom domain with [these instructions](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site).


[^1]: The warped email image is a simple yet effective measure to protect your email address from automated scraping. Web crawlers and bots often harvest email addresses from websites for spam lists. By presenting your email as a slightly distorted image, it remains easily readable for human visitors while being much more difficult for automated systems to recognize and collect. This small step can prevent an increase in the amount of unwanted emails and spam that would come from putting up your email address directly.

[^2]: Some resources for working with Markdown are this [general cheat sheet](https://www.markdownguide.org/cheat-sheet/) and this [Markdown-Cheatsheet repo](https://github.com/lifeparticle/Markdown-Cheatsheet).

[^3]: Welcome/landing page at `index.md`, Research page at `\_portfolio\index.md`, and the Teaching/Links/Contact pages in the `\_pages\` folder at `teaching.md`, `links.md`, and `contact.md`
