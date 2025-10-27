**BOOK RECOMMENDATION SYSTEM:**

This is a GUI-based Book Recommendation application that fetches book data (title, author, publish date, rating, and cover image) using the Google Books API and displays them in a visually styled interface.
It’s primarily an educational or prototype-level project, demonstrating:

Integration of a GUI (tkinter)

Use of an external API (Google Books API)

Dynamic image handling with PIL (Pillow)

**User Search Input:
**
The user types a book name into a search box.

The app sends an HTTP GET request to Google Books API:

https://www.googleapis.com/books/v1/volumes?q=<search_term>&maxResults=5


It fetches up to 5 book results.

**Data Display:**

For each book, it extracts:

title

publisher

publishedDate

authors

averageRating

thumbnail image link
**
Then displays:**

Book title (always shown)

Publish date (optional)

Rating (optional)

Book cover image (resized and shown via Pillow)

**Settings Menu:**

Allows toggling between displaying extra info:

“Publish Date”

“Rating”

Implemented with Tkinter checkbuttons in a dropdown menu.

**Frames Layout:**

There are five display frames for showing up to five recommended books.

Each has subframes for text (title, date, rating) and an image.

Visual Design:

Backgrounds, logo, and buttons are image-based (e.g., Images/background.png, Images/Search.png).

UI is non-resizable and fixed at 1250×700 pixels.
