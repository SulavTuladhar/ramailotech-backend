Project Description:

This project is a full-stack web application for managing blog posts. It includes both the backend and frontend components, implemented using Express JS and React respectively. The backend is built using the FastAPI framework, providing a RESTful API for CRUD operations
on blog posts, categories, and tags. User authentication and authorization are implemented using JSON Web Tokens (JWT). The frontend is developed using React, providing various components/pages for interacting with the blog posts, including listing recent posts, 
displaying post details, creating/updating posts, browsing categories and tags, and managing user authentication.

Backend:
Framework: Express JS
RESTful API: Implemented for CRUD operations on blog posts, categories, and tags.
Blog Post Fields: Title, content, author, creation date, category, and tags.
Relationships: Each blog post belongs to a category and has multiple tags. Each category can have multiple blog posts, and each tag can be associated with multiple blog posts.
Authentication and Authorization: Implemented using JSON Web Tokens (JWT) for securing endpoints and managing user sessions.
Commenting System: Implemented for blog posts, allowing authenticated users to leave comments.

# Backend API Endpoints

## Auth Routes

### Login
- **POST** `/auth/login`
  - Authenticates a user and generates a JWT token.

### Register
- **POST** `/auth/register`
  - Registers a new user.

## User Routes

### Fetch User
- **GET** `/user/`
  - Retrieves user information.

### Update User
- **PUT** `/user/`
  - Updates user information.

### Fetch Owned Blogs
- **GET** `/user/blogs`
  - Retrieves blogs owned by the user.

## Blog Routes

### Fetch All Blogs
- **GET** `/blog/`
  - Retrieves all blogs.

### Create Blog
- **POST** `/blog/`
  - Creates a new blog.

### Search Blog
- **POST** `/blog/search`
  - Searches for blogs.

### Fetch All Tags
- **GET** `/blog/tag`
  - Retrieves all tags.

### Create Tag
- **POST** `/blog/tag`
  - Creates a new tag.

### Delete Tag
- **DELETE** `/blog/tag/:id`
  - Deletes a tag.

### Fetch All Categories
- **GET** `/blog/category`
  - Retrieves all categories.

### Create Category
- **POST** `/blog/category`
  - Creates a new category.

### Delete Category
- **DELETE** `/blog/category/:id`
  - Deletes a category.

### Fetch Blog by Category
- **GET** `/blog/category/:id`
  - Retrieves blogs by category.

### Fetch Blog
- **GET** `/blog/:id`
  - Retrieves a single blog.

### Update Blog
- **PUT** `/blog/:id`
  - Updates a blog.

### Delete Blog
- **DELETE** `/blog/:id`
  - Deletes a blog.

## Comment Routes

### Comment
- **POST** `/comment/:id`
  - Adds a comment to a blog.

### Update Comment
- **PUT** `/comment/:id`
  - Updates a comment.

### Delete Comment
- **DELETE** `/comment/:id`
  - Deletes a comment.
