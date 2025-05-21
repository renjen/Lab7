**Check Your Understanding**

1) I would fit my automated tests within a GitHub Action that runs whenever code is pushed. This ensures that any new code is immediately tested in an automated, consistent way, which helps catch bugs early and supports a continuous integration workflow. It also removes the reliance on developers manually running tests and reduces the chances of human error.

2) Would you use an end-to-end test to check if a function is returning the correct output?  
NO
End-to-end tests are for simulating full user workflows and checking if the application behaves as expected from a user's perspective. If you want to check whether a specific function returns the correct value, you should use a unit test instead.

3) What is the difference between navigation and snapshot mode?**  
- **Navigation mode** simulates a full page load from scratch: it clears caches, fetches all resources, and measures load‐performance metrics (First Contentful Paint, Largest Contentful Paint, Speed Index, Total Blocking Time). It answers “How fast does a new visitor see and interact with this page?”  
- **Snapshot mode** takes the already‐loaded DOM as is (no reload) and audits it for accessibility, best practices, and SEO issues. It does not measure load‐performance or JS interactions—only the static structure and content currently on the page.

1) Three things we could do to improve the CSE 110 shop site based on the Lighthouse results**  
2. **Resize & convert images**  
   - Scale product images down to their actual display size and convert to a next-gen format (WebP or AVIF).  
   - Add lazy‐loading (`<img loading="lazy">`) to defer offscreen images and shave off hundreds of kilobytes.

3. **Add missing `<meta>` tags**  
   ```html
   <!-- in <head> -->
   <meta name="viewport" content="width=device-width, initial-scale=1">
   <meta name="description" content="CSE 110 Shop – demo storefront with 20 sample products">