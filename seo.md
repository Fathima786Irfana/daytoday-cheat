# SEO Optimization Cheatsheet

### **General Steps**

-   Open **Chrome DevTools** → go to the **Lighthouse** tab → click **Analyze Page Load**.
    
-   Based on the report, resolve the suggestions.  

### 1. **Issue: Multiple `<h1>` Tags on the Page**

**Problem:**  Search engines expect a **single `<h1>`** as the main page heading. Using multiple `<h1>` confuses the page hierarchy and lowers SEO scores.

**Solution:** Ensure that only the primary heading uses `<h1>`.  Change all non-primary headings from `<h1>` to a **more appropriate tag** like `<h2>`, `<h3>` or `<p>`.

**For Example:**  
```
 <h1>Find Your Dream Job</h1>        --> Main heading 
 <h2>Why Choose Us</h2>              --> Section heading 
 <p>Fast Delivery</p>                --> Description 
```