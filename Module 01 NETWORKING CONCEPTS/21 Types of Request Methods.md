# Types of Request Methods

## English Version

HTTP request methods, also known as HTTP verbs, define the type of action that a client wants to perform on a server. Each method has a specific purpose and is used for different types of operations. Here are the most common HTTP request methods:

1. **GET**
   - **Purpose:** Retrieves data from the server. It is used to request resources like HTML pages, images, or other files.
   - **Characteristics:** 
     - Requests are idempotent, meaning multiple identical requests will have the same effect as a single request.
     - Typically used for fetching data without modifying the resource.
   - **Example:** Fetching a webpage `https://www.example.com/about`

2. **POST**
   - **Purpose:** Sends data to the server to create or update a resource. Often used for form submissions or file uploads.
   - **Characteristics:** 
     - Requests are not idempotent, meaning multiple identical requests may have different effects.
     - The server processes the request and may change the resource or create a new one.
   - **Example:** Submitting a registration form with user details.

3. **PUT**
   - **Purpose:** Updates an existing resource or creates a new one if it does not exist. It replaces the entire resource with the data provided.
   - **Characteristics:** 
     - Requests are idempotent; sending the same PUT request multiple times will result in the same resource state.
   - **Example:** Updating a user profile with new information.

4. **DELETE**
   - **Purpose:** Deletes a resource from the server.
   - **Characteristics:** 
     - Requests are idempotent; sending the same DELETE request multiple times will result in the resource being deleted.
   - **Example:** Removing a blog post from a website.

5. **PATCH**
   - **Purpose:** Partially updates a resource. Unlike PUT, which replaces the entire resource, PATCH applies partial modifications.
   - **Characteristics:** 
     - Requests are not necessarily idempotent; multiple identical PATCH requests may have different effects.
   - **Example:** Changing the email address in a user profile without altering other details.

6. **HEAD**
   - **Purpose:** Retrieves the headers of a resource without the body. It is similar to GET but does not return the resource content.
   - **Characteristics:** 
     - Useful for checking metadata like content type and length, without downloading the actual resource.
   - **Example:** Checking if a resource exists and obtaining metadata without downloading the full content.

7. **OPTIONS**
   - **Purpose:** Describes the communication options for the target resource. It can be used to determine the supported methods or capabilities of a server.
   - **Characteristics:** 
     - Typically used for discovering allowed methods and features of a resource.
   - **Example:** Finding out which HTTP methods are supported by an API endpoint.

8. **CONNECT**
   - **Purpose:** Establishes a tunnel to a server, often used for SSL/TLS connections through a proxy.
   - **Characteristics:** 
     - Primarily used for establishing secure connections between the client and server.
   - **Example:** Creating an encrypted connection to a secure server.

9. **TRACE**
   - **Purpose:** Echoes the received request back to the client. It is used for diagnostic purposes.
   - **Characteristics:** 
     - Rarely used in practice and often disabled due to security concerns.
   - **Example:** Testing the path that a request takes to reach the server.

## Hinglish Version

HTTP request methods, jo HTTP verbs bhi kahlate hain, define karte hain ki ek client server pe kaunsa action perform karna chahta hai. Har method ka specific purpose hota hai aur alag-alag types of operations ke liye use kiya jata hai. Yahan kuch common HTTP request methods hain:

1. **GET**
   - **Purpose:** Server se data retrieve karta hai. Yeh resources jaise HTML pages, images, ya other files ko request karne ke liye use hota hai.
   - **Characteristics:**
     - Requests idempotent hote hain, yani multiple identical requests ka same effect hoga ek single request ke jaise.
     - Data ko fetch karne ke liye use hota hai bina resource ko modify kiye.
   - **Example:** Webpage `https://www.example.com/about` ko fetch karna.

2. **POST**
   - **Purpose:** Server ko data bhejta hai taaki ek resource create ya update ho sake. Aksar form submissions ya file uploads ke liye use hota hai.
   - **Characteristics:**
     - Requests idempotent nahi hote, yani multiple identical requests ka different effects ho sakte hain.
     - Server request ko process karta hai aur resource ko change ya naya create kar sakta hai.
   - **Example:** User details ke saath registration form submit karna.

3. **PUT**
   - **Purpose:** Existing resource ko update karta hai ya agar resource exist nahi karta to naya create karta hai. Yeh pura resource replace karta hai jo data provide kiya gaya hota hai.
   - **Characteristics:**
     - Requests idempotent hote hain; same PUT request ko multiple times bhejne par same resource state result hota hai.
   - **Example:** User profile ko naye information ke saath update karna.

4. **DELETE**
   - **Purpose:** Server se resource ko delete karta hai.
   - **Characteristics:**
     - Requests idempotent hote hain; same DELETE request ko multiple times bhejne par resource delete ho jata hai.
   - **Example:** Website se ek blog post remove karna.

5. **PATCH**
   - **Purpose:** Resource ko partially update karta hai. PUT ke contrast me, jo pura resource replace karta hai, PATCH partial modifications apply karta hai.
   - **Characteristics:**
     - Requests necessarily idempotent nahi hote; multiple identical PATCH requests ka different effects ho sakte hain.
   - **Example:** User profile me email address ko change karna bina other details ko alter kiye.

6. **HEAD**
   - **Purpose:** Resource ke headers ko retrieve karta hai bina body ke. Yeh GET ke similar hai lekin resource content return nahi karta.
   - **Characteristics:**
     - Metadata jaise content type aur length check karne ke liye useful hai bina actual resource ko download kiye.
   - **Example:** Resource exist karta hai ya nahi aur metadata obtain karna bina full content download kiye.

7. **OPTIONS**
   - **Purpose:** Target resource ke communication options ko describe karta hai. Yeh server ke supported methods ya capabilities ko determine karne ke liye use hota hai.
   - **Characteristics:**
     - Typically allowed methods aur features discover karne ke liye use hota hai.
   - **Example:** API endpoint ke supported HTTP methods ko find out karna.

8. **CONNECT**
   - **Purpose:** Server ke saath ek tunnel establish karta hai, aksar SSL/TLS connections ke liye proxy ke through use hota hai.
   - **Characteristics:**
     - Primarily secure connections establish karne ke liye use hota hai client aur server ke beech.
   - **Example:** Secure server ke saath encrypted connection create karna.

9. **TRACE**
   - **Purpose:** Received request ko client ko echo karta hai. Yeh diagnostic purposes ke liye use hota hai.
   - **Characteristics:**
     - Practically rarely use hota hai aur security concerns ke karan aksar disabled hota hai.
   - **Example:** Request ka path test karna jo server tak pahunchti hai.
