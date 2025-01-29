# mongoDB
Product.find({ 
    category: 'Electronics', 
    price: { $gt: 500 } 
})
.sort({ price: -1 })
.exec((err, products) => {
    if (err) {
        console.log(err);
    } else {
        console.log(products);
    }
});
