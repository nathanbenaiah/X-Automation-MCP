X Automation MCP

This project creates and posts content on X using your niche. It collects information from X, saves what it learns, and writes new posts based on that information. The system can also publish the posts for you. Everything works through an MCP server so any agent that supports MCP can use it.

What the project does

It reads tweets related to a niche you choose.
It creates a short summary so the system understands the niche.
It saves this information in Pinecone.
It uses OpenAI to write new posts.
It can publish the posts on your X account if you want.

Why this is useful

Finding ideas, researching trends, and posting often can take a lot of time.
This project helps you keep your account active without doing everything by hand.

Technology used

Node.js and TypeScript
X API
OpenAI
Pinecone
MCP server

How it works

You choose a niche such as fitness, technology, motivation, or anything else.
The system searches X for tweets in that niche.
It summarizes what people talk about.
It stores useful information in Pinecone so it can be used again later.
It writes new posts from what it has learned.
It can publish the posts automatically.

Setting up the project

Copy the values in the example file named .env.example into a new file called .env.
Add your keys in the correct places.

Example fields:

X_API_KEY
X_API_SECRET
X_ACCESS_TOKEN
X_ACCESS_TOKEN_SECRET
OPENAI_API_KEY
PINECONE_API_KEY
PINECONE_ENVIRONMENT
PINECONE_INDEX_NAME

Running the project

Install the packages with:

npm install

Start the MCP server with:

npm run dev:mcp

You can also run the system directly with:

npm run dev

Main features inside MCP

A tool that creates the knowledge base for the niche
A tool that writes and posts content
A tool that updates the niche information when needed

Project structure

The project is inside folders that follow this idea:

config contains environment settings
services contains API clients for X, OpenAI, and Pinecone
workflows contains the main actions of the system
mcp contains the tools that are exposed to MCP
types contains shared definitions

Who this project is for

People who want automated posting
Developers who want to study MCP
Anyone learning how to connect X, OpenAI, and Pinecone

Future improvements

Support for more niches
Better content quality
Thread creation
A simple web dashboard for control

License

MIT License
