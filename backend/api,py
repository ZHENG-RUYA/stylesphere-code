from flask import Flask, jsonify, request
from models import init_db, Product, Order

app = Flask(__name__)
init_db()

@app.route('/api/products')
def get_products():
    products = Product.query.all()
    return jsonify([p.to_dict() for p in products])

@app.route('/api/order', methods=['POST'])
def create_order():
    data = request.json
    # 订单处理逻辑
    return jsonify({"status": "success"})
