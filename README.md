# LegalEase – Find a Lawyer

LegalEase is a simple web tool that helps people search for lawyers based on their legal needs. It uses AI to understand what the user is looking for and matches them with the most relevant lawyers.

Live: [https://lawyer.sloq.me](https://lawyer.sloq.me)

## What It Does

- Lets users search using plain questions like “divorce lawyer in Mumbai”
- Shows lawyer profiles with their experience and specializations
- Uses AI to understand meaning, not just keywords
- Gives real-time search results instantly

## How It Works

```mermaid
flowchart TD
    A[User enters query] --> B[Gemini AI processes it]
    B --> C[Convert to vector]
    C --> D[Search vector database (PostgreSQL)]
    D --> E[Match relevant lawyers]
    E --> F[Show results to user]
```
## How It Works

1. The user types a query
2. AI processes the query and converts it into a vector
3. The system finds matching lawyers from a database
4. The results are shown in a clean, readable format

## Tech Overview

- **Frontend**: Built with Next.js (React)
- **AI**: Google Gemini + vector embeddings
- **Database**: PostgreSQL with vector search
- **Styling**: Tailwind CSS
- **Deployment**: Vercel
