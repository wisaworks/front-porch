# Front Porch v1 (a fork of [Quartz](https://quartz.jzhao.xyz/))

## Instructions

### Step 1 - Create a copy of the Front Porch Repo

You should see the following when viewing the Front Porch Repo:

![Front Porch Repo](https://github.com/DigitalGardeningCollective/front-porch/blob/main/docs/images/front%20porch%20repo.png)

Click on the "Fork" button. Once done, you should see the following page:

![Fork Page](https://github.com/DigitalGardeningCollective/front-porch/blob/main/docs/images/fork%20creation%20page.png)

Use the following format for your fork's name:

[github-username].github.io

For me, that was joshwingreene.github.io.

I recommend that you keep the "Copy the main branch only" option checked.

### Step 2 - Determine which instructions you will follow

Path A - Set up via GitHub's Codespaces Feature (Recommended for people who are new to GitHub and Technical Concepts)

Path B - Set up yourself (Recommended for Technologists)

### Path A - Set up via GitHub's Codespaces Feature (Recommended for people who are new to GitHub and Technical Concepts)

### Step A.1 - Create a Codespace for your fork

After you have created your fork, you should be presented with a page that looks like the following:

![Example Front Porch](https://github.com/DigitalGardeningCollective/front-porch/blob/main/docs/images/example%20front%20porch.png)

Click on the green "Code" button. You should see the following:

![Menu that shows up after the Code button is clicked](https://github.com/DigitalGardeningCollective/front-porch/blob/main/docs/images/codespace%20cta.png)

Click on the "Create codespace on main" button. This will start up a new codespace for you that's connected to the "main" branch of your front porch. Any changes made here will be seen by people who visit your front porch.

You should see a page that looks like this:

![What your Codespace will look like](https://github.com/DigitalGardeningCollective/front-porch/blob/main/docs/images/initial%20state%20of%20codespace.png)

**Important:** Whenever you want to edit your front porch in the future, you should click on the "Code" button and click on the codespace that you created. The name of your codespace is in the bottom left-hand corner of your codespace. For example, mine is called "humble space winner."

### Step A.2 - Install the necessary packages for your Front Porch

Front Porch is a fork of Quartz. Quartz relies on existing technologies in order to work. We need to install those technologies in order for everything to work properly.

Enter the following command into your codespace's terminal and execute it:

```npm install```

Here are two images that show this command in action:

![npm install is entered into the terminal](https://github.com/DigitalGardeningCollective/front-porch/blob/main/docs/images/npm%20install%20is%20entered%20into%20the%20terminal.png)

![npm install is executed](https://github.com/DigitalGardeningCollective/front-porch/blob/main/docs/images/npm%20install%20is%20executed.png)

### Step A.3 - Spin up a preview of your front porch

In order to see a preview of your front porch, you need to use the following command:

```npx quartz build --serve```

![quartz serve command is executed](https://github.com/DigitalGardeningCollective/front-porch/blob/main/docs/images/quartz%20serve%20command%20is%20executed.png)

Once done, hold down the (Ctrl - Windows/Command - Mac) key on your keyboard and click on the ```https://localhost:8080``` link that's shown in your codespace's terminal. A live preview of your front porch will open in a new tab.

Here's what your terminal will look like when you access the preview (files will be different):

![how the terminal will look when the preview is being accessed](https://github.com/DigitalGardeningCollective/front-porch/blob/main/docs/images/live%20front%20porch%20being%20accessed.png)

### Step A.4 Disclaimer -  I am not a lawyer, and the information provided is not legal advice. Please consult a qualified legal professional for legal advice specific to your situation.

### Step A.4 - Navigate to the LICENSE.txt file in the your codespace's file explorer and add the following line to the top of the file:

All Rights Reserved.

### Step A.5 - Navigate to the quartz.config.ts file and update lines 18 to 60 accordingly

For reference, you can see how I edited [mine](https://github.com/joshwingreene/joshwingreene.github.io/blob/main/quartz.config.ts).

### Step A.6 - Update the images in the static folder

Location of the Static Folder
- `root/quartz/static`

### Step A.7 - Go to Step 3

Scroll down until you see it

### Path B - Set up yourself (Recommended for Technologists)

**Prerequisites**

> "Quartz requires **at least [Node](https://nodejs.org/) v18.14** and `npm` v9.3.1 to function correctly. Ensure you have this installed on your machine before continuing"

### Step B.1 - Clone your fork to your machine

`git clone https://github.com/[github-username]/[github-username].github.io.git`

ex. https://github.com/joshwingreene/joshwingreene.github.io.git

### Step B.2 - Use the terminal in order to navigate to your front porch folder and then run `npm install` in order to install all of the necessary packages. The dependencies of Front Porch v1.0.0 is consistent with the dependencies that Quartz v4.2.3 relies on.

### Step B.3 - Spin up a preview of your front porch

In order to see a preview of your front porch, you need to use the following command:

```npx quartz build --serve```

### Step B.4 Disclaimer -  I am not a lawyer, and the information provided is not legal advice. Please consult a qualified legal professional for legal advice specific to your situation.

### Step B.4 - Navigate to the LICENSE.txt file and add the following line to the top of the file:

All Rights Reserved.

### Step B.5 - Navigate to the quartz.config.ts file and update lines 18 to 60 accordingly

### Step B.6 - Update the images in the static folder

Location of the Static Folder
- `root/quartz/static`

### Step B.7 - Go to Step 3

---

### Step 3 - Follow the following steps from Quartz to host your front porch on github

> 1. Head to “Settings” tab of your forked repository on GitHub and in the sidebar, click “Pages”. Under “Source”, select “GitHub Actions”.

> 2. Commit these changes by doing `npx quartz sync`. This should deploy your site to <github-username>.github.io/<repository-name>.

Whenever you want to update your site, you just need to run `npx quartz sync` after saving your changes.

Reference: [Hosting](https://quartz.jzhao.xyz/hosting#github-pages)
- The deploy.yml file was added for you.

### Step 4 - Add a custom domain

Follow the steps that Quartz provides:

[Custom Domains](https://quartz.jzhao.xyz/hosting#custom-domain)

### Step 5 - Enjoy!

---

## Documentation - Authoring Content

[Authoring Content](https://quartz.jzhao.xyz/authoring-content)

Front Porch supports all of the frontmatter fields that Quartz uses.

Here are the frontmatter fields that are unique to Front Porch:

| Frontmatter Field | Property Type | Description | 
| ----------------- | ------------- | ----------- | 
| growth-stage      | Text          | Specifies the growth stage of the piece (possible values - seedling, budding, evergreen, statue)(case-insensitive) |
| contributions-enabled | Checkbox  | Specifies whether you are fine with people submitting contributions to this piece (ex. additional arguments). You will need to enable "Issues" on your forked repository on GitHub. You can do this by going to Settings and scrolling down to the Features area. The "Issues" checkbox will be there. |
| total-contributions | Number      | The total number of contributions that you have approved and merged into your piece. The contributions-enabled field must be turned on. |
| contributors | List      | The contributors that have gotten one of their contributions for this piece approved. The contributions-enabled field must be turned on. |
| contributor-links | List      | A list of links that direct readers to the website or github profile of each contributor. The order of the links should be consistent with the contributor list. The contributions-enabled field must be turned on. |
| cover-image | Text      | The name and file extension of the image that you want to show up as the cover image for the piece. The image needs to be added to the "item-cover" folder in the "static" folder. |
| cover-image-alt-text | Text      | The alternative text that should be used for the image in the event that a screen reader is being used. The cover-image field needs to be set. |
| team | List      | The people that were on the team (including you). |
| tech | List      | The technology that was used for the project. |
| tools | List      | The tools that were used for the project. |
| duration | Text      | The duration of the project. |
| role | List      | The roles that you had while working on the project. |
