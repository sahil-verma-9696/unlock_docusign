
# How to Create a New Page in Next.js

Follow these simple steps to create a new page in your Next.js project using the `src/app` directory.

## Steps to Create a Page

### 1. Create a Folder for the Page:

- First, navigate to the `app` directory.
- Create a folder inside the `app` directory with the same name as the page you want to create. This will ensure proper routing in Next.js.

Example:
```
src/app/<folder-name>  # Replace <folder-name> with the desired page name
```

### 2. Create a `page.jsx` File:

- Inside the newly created folder, create a file named `page.jsx`.
- Use the following code template to set up the structure of your page.

```jsx
// src/app/<folder-name>/page.jsx

// your imports

const page = () => {
  return (
    <>
      <main className="size-full flex flex-col gap-8 row-start-2 justify-center items-center">
        <h1>Main</h1>
      </main>
      <footer className="row-start-3 flex gap-6 flex-wrap items-center justify-center">
        Footer
      </footer>
    </>
  );
};

export default page;
```

### Explanation of the Code:
- **`main` tag**: Contains the main content of your page, centered using Flexbox for a neat and organized layout.
- **`footer` tag**: Displays the footer content, also centered and responsive.
- **Styling**: This code uses Tailwind CSS classes like `flex`, `gap-8`, and `items-center` for layout and responsiveness.

## Example Directory Structure:

After creating the folder and `page.jsx` file, your project structure should look like this:

```
/src
  /app
    /about                # Folder for the page
      page.jsx            # The page file containing the above template
```

### Routing:
- Next.js will automatically route to this page based on the folder name.
- For example, if the folder name is `about`, the page will be accessible at `http://localhost:3000/about`.

---

Now you're ready to create your page with ease! Feel free to customize the content and layout to fit your needs.


# How to Create a New Component in Next.js
