# kdg

{
    "customerId": "{{random.number(50)}}",
    "transactionAmount": {{random.number(
        {
            "min":10,
            "max":150
        }
    )}},
    "status": "{{random.weightedArrayElement({
        "weights" : [0.8,0.1,0.1],
        "data": ["OK","FAIL","PENDING"]
        }        
    )}}",
    "transactionTime": "{{date.now}}",
    "transactionType": "{{random.arrayElement(["PURCHASE", "WITHDRAWAL", "DEPOSIT"])}}",
    "merchantId": "{{random.number(1000)}}",
    "currency": "{{random.arrayElement(["USD", "EUR", "GBP"])}}",
    "clothingCategory": "{{random.arrayElement(["Shirts", "Pants", "Dresses", "Jackets", "Shoes", "Accessories"])}}",
    "clothingBrand": "{{random.arrayElement(["Nike", "Adidas", "Zara", "H&M", "Gucci", "Prada"])}}",
    "clothingSize": "{{random.arrayElement(["XS", "S", "M", "L", "XL", "XXL"])}}",
    "color": "{{random.arrayElement(["Red", "Blue", "Green", "Black", "White", "Yellow"])}}",
    "season": "{{random.arrayElement(["Spring", "Summer", "Fall", "Winter"])}}"
}
