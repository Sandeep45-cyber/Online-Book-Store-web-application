# Route Reference

This document lists major routes from `index.js` and `routes/adminAuth.js`.

## User Routes

| Method | Path | Purpose |
|---|---|---|
| GET | `/` | Home page with all books |
| GET | `/login` | User login page |
| GET | `/signUp` | User signup form |
| POST | `/auth` | User authentication |
| POST | `/signup` | Register new user |
| GET | `/forgotpassword` | Password reset form |
| PUT | `/updateuser` | Update user password |
| GET | `/about` | About page |
| GET | `/contact` | Contact page |
| GET | `/terms` | Terms page |
| GET | `/privacy` | Privacy page |
| GET | `/sell` | Sell-book page |
| POST | `/sell` | Submit sell-book request with image |
| GET | `/category/:category` | List books by category |
| GET | `/search/:name` | Search books by exact name |
| GET | `/details/:id` | Book details page |
| POST | `/addbook/:cartid` | Add book to cart |
| GET | `/cart/usercart` | View current cart |
| PUT | `/book/:quantity/:id` | Update cart item quantity |
| PUT | `/deleteproduct/:deleteid` | Remove item from cart |
| POST | `/buyproduct/:data` | Place order from cart |
| GET | `/userorders` | View user orders |
| PUT | `/deleteorderproduct/:deleteid` | Cancel/remove ordered item |
| POST | `/updateprofile/:data` | Update user profile |
| POST | `/contactdata/:data` | Save contact query |
| GET | `/:name/logout` | User logout |

## Admin Routes

| Method | Path | Purpose |
|---|---|---|
| GET | `/admin` | Admin login page |
| POST | `/adminauth` | Admin authentication |
| GET | `/dashboard` | Admin dashboard |
| GET | `/orders` | View aggregated user orders |
| GET | `/adminusers` | View/manage admin users |
| POST | `/addadmin/:newadmin` | Create admin user |
| GET | `/categorytype/:category` | Admin view of books by category |
| POST | `/addbook` | Add new book |
| POST | `/updatebook/:bookid` | Update existing book |
| DELETE | `/deleteproduct/:val` | Delete book |
| GET | `/getdetails/:val` | Get book details for edit view |
| GET | `/query` | View contact queries |
| GET | `/:bookId/userOrderCart` | View a user's order/cart data |
| POST | `/updateprofile` | Update admin profile |
| GET | `/logout` | Admin logout |

## Dev/Test Data Route Notes

The following routes appear to be utility routes:

- `GET /form`
- `POST /details`
- `GET /getbooks`
- `PUT /updatebook`
- `DELETE /deletebook`
- `GET /details`

Use them carefully in production.
