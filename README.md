<a href="https://www.llamatutor.com">
  <img alt="Llama Tutor" src="./public/og-image.png">
  <h1 align="center">Llama Tutor</h1>
</a>

<p align="center">
  An open source AI personal tutor. Powered by Llama 3 70B & Together.ai
</p>

[![Deploy with Vercel](https://vercel.com/button)](https://llamatutor-brkd96d3e-nikitas-projects-09319d29.vercel.app/)

## Tech stack

- Llama 3.1 70B from Meta for the LLM
- Together AI for LLM inference
- Next.js app router with Tailwind
- Serper for the search API
- Helicone for observability
- Plausible for website analytics

## Cloning & running

1. Fork or clone the repo
2. Create an account at [Together AI](https://togetherai.link) for the LLM
3. Create an account at [SERP API](https://serper.dev/) or with Azure ([Bing Search API](https://www.microsoft.com/en-us/bing/apis/bing-web-search-api))
4. Create an account at [Helicone](https://www.helicone.ai/) for observability
5. Create a `.env` (use the `.example.env` for reference) and replace the API keys
6. Run `npm install` and `npm run dev` to install dependencies and run locally

## Future Tasks

- [ ] Add a share & copy buttons that folks can click on after convos are generated
- [ ] Add potential follow up questions + new chat at the end of chat page
- [ ] Split the page into two pages and add back the footer
- [ ] Move all my icons into their own typescript file (transform.tools)
- [ ] Add a more detailed landing page with a nice section with the GitHub link
- [ ] Add nice hamburger menu on mobile
- [ ] Try out the generative UI stuff from Vercel
- [ ] Add a nicer dropdown overall

## Getting Started 🚀


### Installation
```
git clone https://github.com/Tokimikichika/llamatutor
cd llamatutor
npm install
```

##### Configuration
1. Copy environment template:

```
cp .example.env .env
```

2. Update .env with your keys:

```
TOGETHER_API_KEY="your_together_key"
SERPER_API_KEY="your_serper_key"
HELICONE_API_KEY="your_helicone_key"
Running Locally
```

3. Running Locally
```
npm run dev
```

4. Open http://localhost:3000 in your browser.


### Deployment 🌐

Vercel (Recommended)
Import your repository to Vercel Dashboard

Add all environment variables from .env

Set build settings:

Build Command: npm run build

Output Directory: .next

Node.js Version: 18.x