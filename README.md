# RESTAURANT REVIEW SYSTEM
This is a simple implementation of a restaurant review system in Python. The system consists of three main classes: `Customer`, `Restaurant`, and `Review`. It mimics the basic functionality of a Yelp-style domain where customers can leave reviews for restaurants.

## Classes
### Customer
The `Customer` class represents an individual who can leave reviews for restaurants.

#### Attributes:

- `given_name`: The given name of the customer.
- `family_name`: The family name of the customer.
- `reviews`: A list of reviews authored by the customer.

#### Methods:
- `given_name()`: Returns the given name of the customer.
- `family_name()`: Returns the family name of the customer.
- `full_name()`: Returns the full name of the customer.
- `all()`: Returns a list of all customer instances.
- `num_reviews()`: Returns the total number of reviews authored by the customer.
- `find_by_name(name)`: Class method that finds the first customer with a given full name.
- `find_all_by_given_name(name)`: Class method that finds all customers with a given given name.
- `add_review(restaurant, rating)`: Adds a new review associated with the customer and a specified restaurant.

### Restaurant
The `Restaurant` class represents a restaurant that can receive reviews.

#### Attributes:

- `name`: The name of the restaurant.
- `reviews`: A list of reviews for the restaurant.

#### Methods:

- `name()`: Returns the name of the restaurant.
- `reviews()`: Returns a list of all reviews for the restaurant.
- `customers()`: Returns a unique list of customers who have reviewed the restaurant.
- `average_star_rating()`: Returns the average star rating for the restaurant based on its reviews.

### Review
The `Review` class represents an individual review left by a customer for a specific restaurant.

#### Attributes:
- `customer`: The customer who left the review.
- `restaurant`: The restaurant being reviewed.
- `rating`: The star rating given in the review.

#### Methods:
- `rating()`: Returns the star rating of the review.
- `customer()`: Returns the customer object for the review.
- `restaurant()`: Returns the restaurant object for the review.

## Example Usage
python
Copy code
customer1 = Customer("John", "Doe")
restaurant1 = Restaurant("Delicious Bites")

### Add a review
customer1.add_review(restaurant1, 4)

### Accessing information
print(customer1.full_name())  # Output: John Doe
print(customer1.num_reviews())  # Output: 1
print(restaurant1.average_star_rating())  # Output: 4.0

## Dependencies
This project does not have external dependencies. It is a standalone Python implementation. Feel free to explore and extend the functionality based on your project requirements.

## How to Run
Clone the repository.
Run the Python script in your preferred environment.

## Contributing
Contributions are welcome! If you have suggestions or find issues, please open an issue or create a pull request.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Author
Mary Mwangi,



