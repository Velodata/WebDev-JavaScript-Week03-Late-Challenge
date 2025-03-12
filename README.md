# 🚀 **Emergency Coding Challenge: Convert Random User API Data into a Table!**

## **Objective:**
The goal of this challenge is to modify an existing project where you fetch random user data from the [Random User API](https://randomuser.me/api/). Instead of displaying a few key details in a user card, you will dynamically create a **table** to list **all** the key-value pairs in the returned JSON data for each user.

## **Challenge Instructions:**

1. **Gender Selection:**  
   The existing HTML contains radio buttons for selecting gender (Male/Female). Keep this functionality intact.

2. **Fetch Data:**  
   When the **"Fetch User"** button is clicked:
   - Make an AJAX request to the Random User API (`https://randomuser.me/api/?gender=male` or `https://randomuser.me/api/?gender=female` based on the selected gender).
   - The data returned should be displayed in a **table** format rather than a card.
   
3. **Table Structure:**
   - The table should have **two columns**:  
     1. **Key** – representing the JSON key (e.g., `name.first`, `location.city`, etc.)
     2. **Value** – the actual data associated with that key.
   - List all the key-value pairs dynamically in the table, no matter how many fields the API returns.

4. **Table Updates:**  
   - Each time a new user is fetched, **replace** the previous table with the new user's data.
   - Ensure that the table is properly formatted and easy to read.

5. **CSS:**  
   - Apply **basic CSS** to make the table readable and well-structured (e.g., adding borders, padding, and styling the header).

---

## **Example:**
For a response like this from the Random User API:
```json
{
  "results": [
    {
      "name": { "first": "John", "last": "Doe" },
      "location": { "city": "New York", "country": "USA" },
      "email": "johndoe@example.com",
      "dob": { "age": 32 }
    }
  ]
}
