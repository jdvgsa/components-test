# Components and Props

## Attributions

- Course Title: CPNT262
- Assignment name: CPNT-262 Assignment 5 - Components and Props
- Author name: John Dagsa
- GH Pages Link: [https://jdvgsa.github.io/components-test/]
- Netlify Pages Link: [https://celadon-quokka-a2f4c3.netlify.app/]

# Search Research Notes

My goal was to find out the reason why my initial repository for this assignment would not deploy correctly on netlify. I followed the steps listed here on this website [https://docs.netlify.com/cli/get-started/]

- First I typed in my terminal [npm install netlify-cli -g]
- Second I typed [netlify init]
- Third I followed the prompts to deploy the website through netlify CLI
- Fourth I authorized my GitHub and linked the repo to my Netlify Account.
- Fifth I deployed the website but it would only show 404 Not Found.

- I then proceeded to read a ton of information and tutorials and also watched youtube videos on deploying a Netlify Website which ended up being extremely outdated as they were uploaded over a year ago.

- Search Term on google [Netlify Page won't deploy] - Link Result [https://answers.netlify.com/t/support-guide-i-ve-deployed-my-site-but-i-still-see-page-not-found/125?utm_source=404page&utm_campaign=community_tracking]
- Useful Keywords [404 Netlify Page Not Found]

One of the solutions it suggests to do is to fix the directory of the repo that it connects to so that Netlify is able to connect to the correct directory. This then led me to my second search term.

- Second Search Term Used on google ["how to change publish directory"] - Link Result [https://docs.netlify.com/configure-builds/overview/]

- Useful Keywords ["Netlify Publish Directory"]

I went to configure my site and followed the instructions, I specifically selected the correct directory and configured the site settings however it would still display 404 Not found on my Netlify page.

- This is my original Netlify Site [https://admirable-cuchufli-dd3341.netlify.app/] which still displays 404 Not Found.

Unfortunately none of the solutions worked, no matter what I tried. I started thinking that it was because Netlify could not access the files because the files were stored in a sub-folder. I tried moving the folders out and re-deploying but that still did not work.

Ultimately to solve the problem, I created a new repository and I copy and pasted my local files into the new repository, followed the redeployment steps and I was finally able to have my assignment rendered on a Netlify site. [https://celadon-quokka-a2f4c3.netlify.app/]



