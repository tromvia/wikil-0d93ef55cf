# Concept walkthrough

Static page. Open `index.html`. Not indexed by search engines (noindex meta tag and robots.txt).

## Connect the Google Form (once)
1. Create a Google Form with two short or long text questions: "Name" and "Picks".
2. Form menu (three dots) > "Get pre-filled link". Type anything in both fields and click "Get link".
3. In the copied link, find `entry.NNNN=` for each field. The first is Name, the second is Picks.
4. Replace `viewform` with `formResponse` in the link's path and drop everything after the `?`. That is `FORM.url`.
5. In `config.js`, fill in `url`, `nameField` (`entry.NNNN`), `picksField` (`entry.NNNN`).
6. Commit and push. Link the form's responses to a Google Sheet from the Form's Responses tab.
