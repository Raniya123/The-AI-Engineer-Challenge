# 🎨 Mental Coach AI - Frontend

Welcome to the most dope mental wellness chatbot frontend you've ever seen! This Next.js app connects you with your very own AI mental coach. 🧠✨

## 🚀 What's This About?

This is a sleek, modern chat interface built with Next.js and TypeScript that talks to our FastAPI backend. It's got all the good stuff:

- 💬 Real-time chat with your AI mental coach
- 🎨 Beautiful gradient design with dark mode support
- 📱 Fully responsive - works great on mobile and desktop
- ⚡ Lightning-fast with Next.js 15
- 🎯 Type-safe with TypeScript

## 🛠️ Tech Stack

- **Next.js 15** - The React framework for production
- **TypeScript** - Because we like our code type-safe
- **Tailwind CSS** - For styling that doesn't make you cry
- **React 19** - The latest and greatest

## 🏃‍♀️ Getting Started

### Prerequisites

- Node.js (v18 or higher)
- npm (comes with Node.js)
- The backend running on `http://localhost:8000`

### Installation

1. **Install dependencies** (if you haven't already):
   ```bash
   npm install
   ```

2. **Make sure your backend is running**:
   - The backend should be running on `http://localhost:8000`
   - Check the main README for backend setup instructions

3. **Start the development server**:
   ```bash
   npm run dev
   ```

4. **Open your browser** and head to:
   ```
   http://localhost:3000
   ```

## 🎮 Available Scripts

- `npm run dev` - Starts the development server on port 3000
- `npm run build` - Creates an optimized production build
- `npm start` - Runs the production build
- `npm run lint` - Runs the linter to keep your code clean

## 🎨 Features

### Chat Interface
- **Message bubbles**: User messages appear in indigo on the right, AI responses in white/gray on the left
- **Loading indicator**: See those cute bouncing dots while the AI is thinking
- **Auto-scroll**: Messages automatically scroll into view
- **Responsive design**: Looks great on any device

### UX Highlights
- **Visual clarity**: High contrast text ensures readability
- **Smooth animations**: Message sending and loading states feel natural
- **Error handling**: Graceful error messages if something goes wrong
- **Disabled states**: Can't spam the send button while loading

## 🚢 Deployment on Vercel

This app is designed to be deployed on Vercel (because it's Next.js and they go together like peanut butter and jelly):

1. **Push your code to GitHub**
2. **Connect your repo to Vercel**
3. **Deploy!** (Vercel auto-detects Next.js apps)

That's it! Vercel handles the build and deployment automatically.

For more details, check out the [Vercel deployment docs](https://vercel.com/docs).

## 🤝 API Integration

The frontend connects to the backend at `http://localhost:8000/api/chat` with:

```typescript
{
  message: string  // Your message to the AI
}
```

And receives:

```typescript
{
  reply: string  // The AI's response
}
```

## 🎭 Customization

Want to make it your own? Here's what you can tweak:

- **Colors**: Check out `tailwind.config.ts` to change the color scheme
- **AI personality**: Modify the backend's system prompt
- **Layout**: Components are in `app/page.tsx` - go wild!
- **Styles**: Global styles in `app/globals.css`

## 🐛 Troubleshooting

**Chat not working?**
- Make sure the backend is running on port 8000
- Check your browser console for errors
- Verify your OPENAI_API_KEY is set in the backend

**Styling looks weird?**
- Try `npm install` again
- Make sure Tailwind is configured correctly

**Port 3000 already in use?**
- Change the port in `package.json`: `"dev": "next dev -p 3001"`

## 📚 Learn More

- [Next.js Documentation](https://nextjs.org/docs)
- [Tailwind CSS](https://tailwindcss.com/docs)
- [TypeScript](https://www.typescriptlang.org/docs)

## 💪 Contributing

Found a bug? Want to add a feature? PRs are welcome! Just make sure to:
- Test your changes locally
- Keep the code clean and documented
- Follow the existing code style

---

Built with ❤️ for the AI Engineer Challenge