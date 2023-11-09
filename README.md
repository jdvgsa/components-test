# Components and Props

## Attributions

- Course Title: CPNT262
- Assignment name: CPNT-262 Assignment 5 - Components and Props
- Author name: John Dagsa
- GH Pages Link: [https://jdvgsa.github.io/components-test/]
- Netlify Pages Link: [https://celadon-quokka-a2f4c3.netlify.app/]

# Search Research Notes

My goal was to find out the reason why my initial repository [https://github.com/jdvgsa/componnets-props] for this assignment would not deploy correctly on netlify. I followed the steps listed here on this website [https://docs.netlify.com/cli/get-started/]

- First I typed in my terminal [npm install netlify-cli -g]
- Second I typed [netlify init]
- Third I followed the prompts to deploy the website through netlify CLI
- Fourth I authorized my GitHub and linked the repo to my Netlify Account.
- Fifth I deployed the website but it would only show 404 Not Found.

- I then proceeded to read a ton of information and tutorials and also watched youtube videos on deploying a Netlify Website which ended up being extremely outdated as they were uploaded over a year ago.

- Search Term on google ["Netlify Page won't deploy"] - Link Result [https://answers.netlify.com/t/support-guide-i-ve-deployed-my-site-but-i-still-see-page-not-found/125?utm_source=404page&utm_campaign=community_tracking]
- Useful Keywords [404 Netlify Page Not Found] This gave more useful information and got me to the link above directly on the first search result.
- Unuseful Keywords / Search Term ["Why won't my netlify page deploy with my GitHub Repo?"] This makes the search results vague as results show individual cases and links to some forums.

One of the solutions it suggests to do is to fix the directory of the repo that it connects to so that Netlify is able to connect to the correct directory. This then led me to my second search term.

- Second Search Term Used on google ["how to change publish directory"] - Link Result [https://docs.netlify.com/configure-builds/overview/]

- Useful Keywords ["Netlify Publish Directory"]

I went to configure my site and followed the instructions, I specifically selected the correct directory and configured the site settings however it would still display 404 Not found on my Netlify page.

- This is my original Netlify Site [https://admirable-cuchufli-dd3341.netlify.app/] which still displays 404 Not Found.

Unfortunately none of the solutions worked, no matter what I tried. I started thinking that it was because Netlify could not access the files because the files were stored in a sub-folder. I tried moving the folders out and re-deploying but that still did not work.

Ultimately to solve the problem, I created a new repository and I copy and pasted my local files into the new repository, followed the redeployment steps and I was finally able to have my assignment rendered on a Netlify site. [https://celadon-quokka-a2f4c3.netlify.app/]

--------------------------------------------------------------------------------------

My second goal which remains unsolved is why my TailWind won't work with my project.

- Search Term used ["TailwindCSS Sveltekit"] which prompts this link [https://tailwindcss.com/docs/guides/sveltekit] as the first option.

I followed the steps in the installation process,
Step 1:
- npm install -D tailwindcss
- npx tailwindcss init

Step 2: Configure your template paths
Add the paths to all of your template files in your tailwind.config.js file.

I pasted this code [/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}] on my tailwind.config.js as instructed.

The rest of the steps listed on the site was followed [https://tailwindcss.com/docs/installation].

None of the solutions worked and ultimately I gave up on tailwind as assignment does not specifically require. So the solution I came up with was I decided to just style my page with plain old CSS.



