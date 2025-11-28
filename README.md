Eros - AI-Powered Holistic Well-Being Platform:-

•	Build a comprehensive multi-feature wellness application with a centralized dashboard that connects 8 AI-powered modules for mental health, sustainability, learning, nutrition, code review, finance, volunteering, and emotional healing—all wrapped in a beautiful dark-themed interface with smooth animations.
Key UI & Components:-

•	Homepage: Animated floating doodles (hearts, brains, leaves, code brackets, coins, handshakes) with hero section, feature highlights, and CTA button leading to authentication

•	Authentication Flow: Login/signup pages with email/password + Google OAuth, form validation, loading states, and smooth transitions to dashboard

•	Central Dashboard: 8 interactive feature cards in responsive 2x4 grid layout, each with icon, title, description, and "Open" button that navigates to dedicated feature page

•	Feature Pages: Each of the 8 modules gets its own full page with specialized UI (chat interfaces, input forms, data visualizations, code editors, calendars, etc.) and a persistent "Return to Dashboard" button in top-right

•	Navigation System: Bottom nav bar for mobile (Dashboard/Profile/Settings), breadcrumb trail for desktop, smooth page transitions with Framer Motion

Key Features & Functionality:-

•	Mental Health Companion: Voice/text input for daily check-ins, AI emotion analysis, personalized coping exercises, mindfulness audio player, mood tracking charts with weekly insights

•	Sustainability Tracker: Input forms for travel/shopping/energy data, real-time carbon footprint calculator, AI-generated reduction tips with impact scores, progress charts and community leaderboard

•	Smart Learning Buddy: Subject selector with difficulty levels, AI-generated study plans, adaptive quizzes with detailed explanations, progress tracking with spaced repetition and mastery badges

•	AI Recipe Creator: Ingredient input with dietary preferences, instant recipe generation, weekly meal planner, auto-generated grocery lists, nutrition breakdowns, cooking timers, favorites system

•	Code Review Assistant: Multi-language code snippet input, AI bug/security/optimization detection, one-click fix application, before/after comparison view, integrated dark mode code editor

•	Finance Advisor: Bank connection mockup, spending categorization, AI budget recommendations, goal setting, investment suggestions, net worth tracker, financial scenario simulations

•	Volunteering Hub: Location and skills input, AI matching algorithm for nearby opportunities, compatibility scores, event calendar with RSVP system, impact tracking dashboard

•	Empathy Chatbot: Conversational AI for forgiveness/healing, emotion detection from text/voice input, guided empathy exercises, relationship advice, session history with progress insights

•	Cross-Cutting Features: Voice input everywhere using Web Speech API, achievement badges system, daily motivational quotes, shareable progress reports, onboarding tour, heart particle effects on positive interactions


Style & Technical Approach:-

•	Color Palette: Deep indigo background (#1e1b4b), rich purple accents (#6d28d9), emerald green success states (#10b981), amber warnings (#f59e0b), soft white text (#f8fafc), dark slate cards (#0f172a), lavender borders (#a78bfa)

•	Tech Stack: Vite + React with Tailwind CSS and shadcn/ui components, Framer Motion for animations, Zustand for state management, OpenAI/Claude API integration (with mock fallbacks)

•	Animation Strategy: Smooth 0.3s page transitions, floating doodle animations on homepage, card hover effects, form input animations, loading skeletons everywhere, particle effects for positive feedback

•	Responsive Design: Mobile-first approach with bottom navigation on small screens, desktop breadcrumbs and expanded layouts, all feature pages adapt gracefully across breakpoint

•	Production Polish: PWA capabilities, error boundaries, SEO metadata, offline mode for core features, dark theme toggle (default dark), persistent "Return to Dashboard" button on all feature pages


##Implementation Note: Start with the homepage, authentication flow, and dashboard hub first. Then build out 2-3 feature pages as proof of concept before completing all 8 modules. Use mock AI responses initially, then integrate real API calls with proper error handling and rate limiting.# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
export default {
  // other rules...
  parserOptions: {
    ecmaVersion: 'latest',
    sourceType: 'module',
    project: ['./tsconfig.json', './tsconfig.node.json'],
    tsconfigRootDir: __dirname,
  },
}
```

- Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
- Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and add `plugin:react/recommended` & `plugin:react/jsx-runtime` to the `extends` list
