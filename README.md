Narrative Report:  PHP Class Implementation for Product and Movie Data Management
 
This report analyzes two PHP code examples (Activity 1 and Activity 2), both demonstrating the creation and utilization of classes to represent and manage product and movie data, respectively.  The report assesses the code's structure, functionality, and potential areas for improvement.
 
Activity 1:  The  Product  Class
 ![image](https://github.com/user-attachments/assets/518eba47-e97e-4228-913b-c09cb5422e68)
![image](https://github.com/user-attachments/assets/ce44dc05-3473-44e3-a03b-9752a6220625)

Activity 1 introduces a  Product  class designed to encapsulate product attributes.  The class utilizes public properties ( Brand ,  Price ,  Size ,  Quality ,  Stock ), which, while simplifying access, compromises data integrity.  For enhanced data security and maintainability,  private properties paired with getter and setter methods are recommended. This approach would allow for controlled access and potential data validation.
 
The class includes two core methods:
 
-  setProduct() : This constructor-like method initializes the product's properties.  The argument order directly maps to the property order within the class.  This approach is prone to errors; using named parameters or an associative array would significantly improve readability and reduce the risk of mismatched arguments.
-  getProductInfo() : This method returns a formatted string containing the product's details.  The use of newline characters ( \n ) enhances readability. However, the mapping of  Size  to "Category" and  Quality  to "Description" might not be universally intuitive and could benefit from more descriptive labels or a more flexible approach to attribute naming.
 
The provided example instantiates a  Product  object representing a laptop and prints its details. The output is clear and functional, but the labeling could be improved for better clarity.
 
Activity 2: The  Movie  Class
 ![image](https://github.com/user-attachments/assets/2149043f-b502-4e7e-b27a-8aab3ddcd288)
![image](https://github.com/user-attachments/assets/ac22c113-c6f2-4c8e-bda9-0f71dccda27a)

Activity 2 presents a  Movie  class, mirroring the structure of Activity 1 but for movie data.  It uses public properties ( title ,  director ,  releaseYear ,  genre ,  rating ), again sacrificing data encapsulation for simplified access.  The same recommendation for private properties with getters and setters applies here.
 
The  Movie  class includes:
 
-  setMovie() : This method initializes the movie object's properties.  Similar to  setProduct() , the argument order is crucial and should be improved using named parameters or an associative array for better readability and error prevention.
-  getMovieInfo() : This method returns a formatted string displaying the movie's details.  The output is a single, well-structured sentence, clearly presenting all attributes.
 
The example creates a  Movie  object for "Avengers Endgame" and prints its information. The output is concise and easily understandable.
 
Overall Assessment and Recommendations
 
Both activities demonstrate fundamental OOP concepts in PHP, specifically class creation and object instantiation.  The consistent use of methods for data manipulation promotes code organization.  However, the reliance on public properties is a significant weakness.  Adopting private properties with getter and setter methods, along with the use of named parameters or associative arrays in the initialization methods, would significantly enhance data security, maintainability, and code readability.  Further improvements could include more descriptive property names and more flexible output formatting in the  getProductInfo()  method.  These modifications would significantly strengthen the code's robustness and adhere to best practices in object-oriented programming.

Submitted by: Ashley arce
khaizer reyes
