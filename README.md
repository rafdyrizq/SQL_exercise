CREATE TABLE coffee_transactions (
    transaction_id INT PRIMARY KEY AUTO_INCREMENT,
    transaction_date DATETIME NOT NULL,
    customer_name VARCHAR(50) NOT NULL,
    menu_item VARCHAR(50) NOT NULL,
    item_category VARCHAR(20) NOT NULL,
    quantity INT NOT NULL,
    item_price DECIMAL(10,2) NOT NULL,
    total_amount DECIMAL(10,2) NOT NULL,
    payment_method ENUM('Cash', 'Debit Card', 'Credit Card', 'Mobile Payment'),
    barista_name VARCHAR(50)
);

-- Insert 30 transaksi dengan nama pemain bola dan barista
INSERT INTO coffee_transactions (transaction_date, customer_name, menu_item, item_category, quantity, item_price, total_amount, payment_method, barista_name) VALUES
('2023-10-01 08:15:00', 'Lionel Messi', 'Latte', 'Coffee', 1, 30.00, 30.00, 'Debit Card', 'Jordan'),
('2023-10-01 09:30:00', 'Cristiano Ronaldo', 'Cappuccino', 'Coffee', 1, 28.00, 28.00, 'Cash', 'Kevin'),
('2023-10-01 10:45:00', 'Neymar Jr', 'Iced Coffee', 'Coffee', 2, 23.00, 46.00, 'Credit Card', 'Stephen'),
('2023-10-01 11:20:00', 'Kylian Mbappe', 'Cold Brew', 'Coffee', 1, 25.00, 25.00, 'Mobile Payment', 'Jordan'),
('2023-10-01 12:30:00', 'Robert Lewandowski', 'Matcha Latte', 'Tea', 1, 29.00, 29.00, 'Debit Card', 'Kevin'),
('2023-10-01 14:15:00', 'Kevin De Bruyne', 'Americano', 'Coffee', 2, 22.00, 44.00, 'Cash', 'Stephen'),
('2023-10-01 15:45:00', 'Mohamed Salah', 'Croissant', 'Food', 1, 25.00, 25.00, 'Mobile Payment', 'Jordan'),
('2023-10-01 16:30:00', 'Erling Haaland', 'Mocha', 'Coffee', 1, 32.00, 32.00, 'Credit Card', 'Kevin'),
('2023-10-02 08:20:00', 'Virgil van Dijk', 'Green Tea', 'Tea', 1, 22.00, 22.00, 'Debit Card', 'Stephen'),
('2023-10-02 09:45:00', 'Harry Kane', 'Sandwich', 'Food', 1, 40.00, 40.00, 'Cash', 'Jordan'),

('2023-10-02 10:30:00', 'Karim Benzema', 'Espresso', 'Coffee', 2, 18.00, 36.00, 'Mobile Payment', 'Kevin'),
('2023-10-02 12:15:00', 'Luka Modric', 'Chocolate Cake', 'Food', 1, 35.00, 35.00, 'Credit Card', 'Stephen'),
('2023-10-02 13:45:00', 'Sadio Mane', 'Latte', 'Coffee', 1, 30.00, 30.00, 'Debit Card', 'Jordan'),
('2023-10-02 15:00:00', 'Son Heung Min', 'Bagel', 'Food', 2, 22.00, 44.00, 'Cash', 'Kevin'),
('2023-10-02 16:20:00', 'Jude Bellingham', 'Muffin', 'Food', 1, 18.00, 18.00, 'Mobile Payment', 'Stephen'),
('2023-10-03 08:10:00', 'Toni Kroos', 'Americano', 'Coffee', 1, 22.00, 22.00, 'Credit Card', 'Jordan'),
('2023-10-03 09:30:00', 'Thibaut Courtois', 'Cappuccino', 'Coffee', 1, 28.00, 28.00, 'Debit Card', 'Kevin'),
('2023-10-03 11:45:00', 'Antoine Griezmann', 'Matcha Latte', 'Tea', 2, 29.00, 58.00, 'Cash', 'Stephen'),
('2023-10-03 13:15:00', 'Marcus Rashford', 'Iced Coffee', 'Coffee', 1, 23.00, 23.00, 'Mobile Payment', 'Jordan'),
('2023-10-03 14:30:00', 'Bukayo Saka', 'Cold Brew', 'Coffee', 1, 25.00, 25.00, 'Credit Card', 'Kevin'),

('2023-10-03 15:45:00', 'Phil Foden', 'Latte', 'Coffee', 2, 30.00, 60.00, 'Debit Card', 'Stephen'),
('2023-10-03 16:50:00', 'Bernardo Silva', 'Mocha', 'Coffee', 1, 32.00, 32.00, 'Cash', 'Jordan'),
('2023-10-04 08:30:00', 'Rúben Dias', 'Chamomile Tea', 'Tea', 1, 20.00, 20.00, 'Mobile Payment', 'Kevin'),
('2023-10-04 10:15:00', 'Rodri', 'Croissant', 'Food', 1, 25.00, 25.00, 'Credit Card', 'Stephen'),
('2023-10-04 11:30:00', 'Guest', 'Espresso', 'Coffee', 1, 18.00, 18.00, 'Cash', 'Jordan'),
('2023-10-04 13:00:00', 'Guest', 'Green Tea', 'Tea', 1, 22.00, 22.00, 'Debit Card', 'Kevin'),
('2023-10-04 14:45:00', 'Vinicius Junior', 'Sandwich', 'Food', 1, 40.00, 40.00, 'Mobile Payment', 'Stephen'),
('2023-10-04 16:00:00', 'Federico Valverde', 'Muffin', 'Food', 2, 18.00, 36.00, 'Credit Card', 'Jordan'),
('2023-10-04 17:15:00', 'Pedri', 'Americano', 'Coffee', 1, 22.00, 22.00, 'Cash', 'Kevin'),
('2023-10-04 17:45:00', 'Gavi', 'Chocolate Cake', 'Food', 1, 35.00, 35.00, 'Debit Card', 'Stephen');
