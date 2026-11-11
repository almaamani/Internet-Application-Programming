# Web Development Exam Answers
b) CSS Box Model Explanation and Product Card Layout
The CSS Box Model is a foundational concept that describes how HTML elements are rendered on a web page. It consists of four concentric rectangular areas:

Content: The innermost area where text or images are displayed. (For a product card, this would be the product image and title).

Padding: The transparent space directly around the content, pushing the inner content away from the border. (Used in product cards to give the text breathing room away from the edges).

Border: The line that surrounds the padding and content. (Could be used to give the product card a distinct outline).

Margin: The outermost transparent space that separates the element from other elements on the page. (Used to create spacing between multiple product cards on an e-commerce grid).

d) Two Ways of Applying CSS Styles to an HTML Document
The prompt actually mentions three methods, but asks to analyze two and recommend one for a large portal.

Inline CSS: Styles applied directly inside an HTML tag using the style attribute.

Internal (Embedded) CSS: Styles placed inside a <style> tag within the <head> section of a specific HTML document.
(The third method, External CSS, involves linking a separate .css file).

Recommendation for a large multi-page government portal:
The most appropriate method is External CSS.
Justification: A government portal will have many pages. External CSS allows for a single stylesheet to control the look of the entire website. If a style needs updating (e.g., changing the national colors), it only needs to be changed in one file, ensuring consistency and reducing redundancy. It also allows the browser to cache the CSS file, improving page load times.

e) Identifying and Correcting Errors in the HTML Snippet
(Note: The exact snippet has a typo in the image, <lInput instead of <input)

Error 1: <lInput Type=text name=studentName>

Correction: <input type="text" name="studentName">

Reason: HTML tags are case-insensitive but standard convention dictates lowercase. There is a typo (lInput instead of input), and attributes should be enclosed in quotes.

Error 2: Radio button naming inconsistency (name="gender" vs name="sex").

Correction: Both should be <input type="radio" name="gender" value="Male"> and <input type="radio" name="gender" value="Female">.

Reason: For radio buttons to function as a group where a user can only select one option, they must share the exact same name attribute.

Error 3: <input type=submit value=Register> (Unquoted attributes).

Correction: <input type="submit" value="Register">

Reason: While some browsers forgive unquoted attributes, it is invalid HTML and can cause bugs. Attribute values should always be wrapped in quotation marks.

Page 2 Answers
Question 2b) Three Types of Lists in HTML5
Ordered List (<ol>): Used for sequential or ranked items.

Scenario: Displaying step-by-step instructions for setting up an online banking account, or ranking the top 10 most visited tourist sites in Kenya.

Unordered List (<ul>): Used for items where order does not matter.

Scenario: Listing navigation menu links on a website header, or listing the ingredients required for a recipe.

Description List (<dl>): Used to pair terms with their definitions or descriptions (using <dt> and <dd>).

Scenario: Creating a glossary of terms, a frequently asked questions (FAQ) section, or displaying product specifications (e.g., Term: "RAM"; Description: "16GB").

Question 2c) Absolute vs. Relative Hyperlinks
Absolute Hyperlink: Contains the full URL, including the protocol (http/https) and domain name (e.g., https://www.centralbank.go.ke).

Usage in Bank Intranet: Should be used when linking to websites outside the bank's internal network (e.g., linking to the Central Bank of Kenya's public site or a government regulatory site).

Relative Hyperlink: Points to a file relative to the current document's location, omitting the domain name (e.g., href="forms/loan-application.html").

Usage in Bank Intranet: Should be used for all internal navigation within the intranet portal itself. This ensures links still work if the bank changes its domain name or moves servers.

Question 2d) Consequences of Missing alt Text
The alt (alternative text) attribute provides a text description of an image if the image fails to load, and is crucial for screen readers. Consequences for a public health website missing this:

Visually Impaired Users: Screen readers will either skip the image entirely or read the file name (e.g., "image_001.jpg"), denying blind users access to critical health information conveyed in graphics.

Users with Slow Internet: If users have poor connectivity and the images fail to load (common in rural areas), they will see empty boxes with no context about what the image was supposed to show.

SEO (Search Engine Optimization): Search engines use alt text to understand image content. Missing it lowers the site's ranking for relevant health-related searches, making it harder for citizens to find the information.

Accessibility Compliance: Government and health sites often have legal obligations to meet accessibility standards (like WCAG). Missing alt text makes the site non-compliant and vulnerable to legal complaints.
