Installation

Clone the repository:

git clone https://github.com/yourusername/my_ecommerce_api.git
cd my_ecommerce_api

Set up a virtual environment:
python3 -m venv venv


Activate the virtual environment:
For macOS/Linux:
source venv/bin/activate

For Windows:
venv\Scripts\activate

Install dependencies:
pip install -r requirements.txt

Initialize the database:
python run.py init-db

Run the application:
python run.py

The application will run on http://localhost:5000/.

API Endpoints
Get all products: GET /products
Get a product by ID: GET /products/<int:product_id>
Create a new product: POST /products
Requires JSON body: { "name": "string", "description": "string", "price": "float" }
Update a product: PUT /products/<int:product_id>
Requires JSON body: { "name": "string", "description": "string", "price": "float" }
Delete a product: DELETE /products/<int:product_id>