Certainly! Here’s a focused, clear **README.md** for your JSON Server backend repo, assuming it serves as the headless API for your React story app.

```markdown
# 📖 Mystic Stories JSON Server API

Simple RESTful backend API for the [Mystic Stories App](https://kay-story-book-app.netlify.app).  
Powered by [JSON Server](https://github.com/typicode/json-server) and deployed on [Render.com](https://render.com/).

---

## 🌐 Live API

- **Base URL:** `https://m2-project-json-server.onrender.com`

---

## 📚 What Is This?

A fake API backend to support story CRUD operations in a decoupled, modern web app.
- Stores stories as JSON objects (with cover images, genres, etc)
- Instantly deployable/forkable—no login or database config needed
- Ideal for rapid prototyping, hackathons, or frontend demos

---

## 🗄️ API Endpoints

| Method | Endpoint        | Function             |
|--------|----------------|----------------------|
| GET    | `/stories`     | Get all stories      |
| GET    | `/stories/:id` | Get single story     |
| POST   | `/stories`     | Create a new story   |
| PUT    | `/stories/:id` | Update a story       |
| DELETE | `/stories/:id` | Delete a story       |

---

## 📝 Story Object Example

```
{
  "id": "uuid-string",
  "title": "The Mystic Sword",
  "description": "A tale of ancient power.",
  "content": "Full story text here...",
  "coverImage": "https://res.cloudinary.com/your-cloud/image/upload/...",
  "status": "published",
  "genres": ["Fantasy", "Adventure"],
  "createdAt": "2024-06-26T13:22:00.000Z",
  "updatedAt": "2024-06-26T13:22:00.000Z"
}
```

---

## 🚀 Local Development

1. **Install JSON Server:**
   ```
   npm install -g json-server
   ```
2. **Create/Edit `db.json`:**
   ```
   {
     "stories": []
   }
   ```
3. **Run the server:**
   ```
   json-server --watch db.json --port 3001
   ```
   Now you can send API requests to `http://localhost:3001/stories`.

---

## 🌍 Deployment

- **Hosted on [Render.com](https://render.com/docs/deploy-json-server)**
- API auto-redeploys on db.json changes (if connected via Git)
- You can fork, duplicate, or redeploy your own copy as needed

---

## 🙏 Credits

- [typicode/json-server](https://github.com/typicode/json-server)
- [Render.com Community Examples](https://render.com/docs/deploy-json-server)

---

## 📝 License

This project is licensed under the [MIT License](./LICENSE).

---

> **Note:** This repo contains only API and data (no frontend).  
For the React app, see: [Mystic Stories App Frontend Repo](https://github.com/yourusername/stories-app)
