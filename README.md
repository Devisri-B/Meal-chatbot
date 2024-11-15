# Meal chatbot
The Meal Chatbot offers an intuitive solution for discovering and filtering recipes based on user-defined criteria. It utilizes both an internal dataset and the Spoonacular API to provide quick and accurate responses. Users can search for recipes based on ingredients, recipe names, preparation times, cuisines, and more.

## Features

- **Hybrid Search Approach**: Combines an internal dataset search using regular expressions and spaCy NLP with external API calls to the Spoonacular API when needed.
- **User-Friendly Interface**: Accessible via a web-based chat interface with an easy-to-use design.
- **Dynamic Query Handling**: Users can search for recipes based on different criteria such as ingredients, cuisine, preparation time, etc.
- **Real-Time Responses**: Provides immediate suggestions and feedback based on user inputs.
## How It Works

- **Internal Dataset Search**: When a user makes a query, the chatbot first attempts to find a match in the internal dataset using:
- **Regular Expressions**: To quickly search and match patterns in user queries.
- **spaCy NLP**: To enhance query understanding and extract named entities, improving the matching process with dataset entries.
- **Spoonacular API Integration**: If the internal search fails to find a suitable match, the chatbot sends a request to the Spoonacular API to fetch relevant recipes. This ensures a comprehensive and robust user experience by providing a wide range of recipes when the internal data is insufficient.
## Usage Instructions

- Clone the repository:```python git clone <repository-url> ```
- Install dependencies: ```python pip install -r requirements.txt ```
- Configure your Spoonacular API key in meal_chatbot.py.
- Start the backend server: python meal_chatbot.py
- Open the chat_interface.html file in your web browser.
- Interact with the chatbot by typing queries related to recipes, and get instant suggestions.
## Chatbot Capabilities with example queries

#### Ingredient-Based Queries
- Search for recipes using specific ingredients you have or want to use.
    -  ⁠"What recipes can I make with chicken and spinach?"  
    - ⁠ "Do you have recipes with potatoes, cheese, and garlic?"  
    -  ⁠"Can I get a recipe with just eggs and bread?"
#### *General Recipe Questions*  
- Find meal ideas tailored to your needs, from dinner options to healthy or beginner-friendly recipes
  -  ⁠"Can I get a recipe for dinner?"  
  -  ⁠"What's a good recipe for beginners?"  
  -  ⁠"What can I make with ingredients I already have?"  

#### *Dietary Restrictions or Preferences*  
- Get recipes tailored to specific dietary needs, such as gluten-free, vegan, or keto
  - "Can I get gluten-free recipes?"  
  -  ⁠"Can I get a vegan burger recipe?"  
  -  ⁠"What recipes are good for a keto diet?"  

#### *Time-Sensitive Questions*  
- Find recipes that match your available cooking time, from quick meals to slow-cooked dishes
    - "Can I get a recipe that takes less than 20 minutes?"
    - ⁠"Do you have quick dessert recipes?"
    -  ⁠"What recipes can I make in under an hour?"

#### *Recipe Name-Based Questions*  
- Retrieve recipes by their name or by popular recipe categories
    - ⁠"Can I get a recipe for pancakes?"
    -   ⁠"What is the best recipe for biryani?"
    - "Can you share a recipe for lasagna?"

#### *Exclusion-Based Questions*  
- Get recipes that exclude specific ingredients based on your preferences
    - ⁠"Can I get a cake recipe without eggs?"
    - ⁠"Do you have a pasta recipe without tomatoes?"
    - ⁠"Can I get a salad recipe without nuts?"  

#### *Meal Type-Based Questions*  
- Discover recipes based on meal types, such as breakfast, lunch, dinner, or snacks.
    - ⁠"What are some easy breakfast recipes?"
    -  ⁠"Can I get lunch ideas for work?"
    -   ⁠"What are some light dinner recipes?"
    - "Can you suggest some snacks for a party?"  

#### *Special Occasion or Seasonal Questions*  
- Find recipes perfect for special occasions or seasonal celebrations
    - ⁠"What are some good recipes for Thanksgiving?"
    - ⁠  ⁠"Can I get Christmas dessert ideas?"  
  -  ⁠"What are some summer salad recipes?"
  -   "Do you have recipes for Valentine's Day?"  

#### *Cooking Technique-Based Questions* 
- Get recipes based on your preferred cooking method, like baking or grilling
  -  ⁠"What are some recipes I can bake?"  
  -  ⁠"Can I get a recipe that requires no cooking?"  
  -  ⁠"Do you have recipes for grilling?"
  -   "What recipes can I make with a slow cooker?"  

## File Structure

- meal_chatbot.py: The backend logic that handles user queries, searches the internal dataset using regular expressions and spaCy, and interacts with the Spoonacular API as needed.
- chat_interface.html: The front-end interface for user interactions with the chatbot.

## Technical Details

- Backend: Built using Flask, which handles user requests and responses, as well as interactions with the internal dataset and the Spoonacular API.
- Internal Dataset Search: Uses regular expressions for pattern matching and spaCy NLP for understanding and extracting relevant entities.
- API Integration: When the internal search yields no results, a request is sent to the Spoonacular API to fetch relevant recipes.
- Frontend: Provides a chat-based interface using HTML, CSS, and JavaScript for a dynamic user experience.

## Contributing

Contributions are welcome! Please open issues or submit pull requests to suggest improvements or new features.


