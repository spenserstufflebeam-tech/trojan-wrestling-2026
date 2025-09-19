# trojan-wrestling-2026
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trojan Wrestling T-Shirt Pre-Order</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #990000 0%, #770000 100%);
            color: #333;
            line-height: 1.6;
            padding: 20px;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
        }
        
        .container {
            max-width: 900px;
            width: 100%;
            background-color: #fff;
            box-shadow: 0 0 20px rgba(0,0,0,0.2);
            border-radius: 10px;
            overflow: hidden;
        }
        
        header {
            background: linear-gradient(135deg, #1a1a1a 0%, #333 100%);
            color: white;
            text-align: center;
            padding: 30px 20px;
            position: relative;
        }
        
        .logo {
            font-size: 40px;
            margin-bottom: 10px;
            color: #990000;
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            color: white;
        }
        
        .subtitle {
            font-size: 1.2rem;
            color: #ccc;
            max-width: 600px;
            margin: 0 auto;
        }
        
        .team-name {
            color: #990000;
            font-weight: bold;
        }
        
        .form-content {
            padding: 30px;
        }
        
        .instructions {
            background-color: #fff8e1;
            padding: 20px;
            border-left: 4px solid #ffc107;
            margin-bottom: 30px;
            border-radius: 4px;
        }
        
        .instructions h3 {
            color: #ff9800;
            margin-bottom: 10px;
        }
        
        .form-section {
            margin-bottom: 30px;
            padding: 20px;
            border-radius: 8px;
            background-color: #f9f9f9;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        
        h2 {
            color: #990000;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 2px solid #ddd;
            display: flex;
            align-items: center;
        }
        
        h2 i {
            margin-right: 10px;
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        label {
            display: block;
            margin-bottom: 8px;
            font-weight: bold;
            color: #555;
        }
        
        input[type="text"],
        input[type="email"],
        input[type="tel"],
        select,
        textarea {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 6px;
            font-size: 16px;
            transition: border-color 0.3s;
        }
        
        input:focus,
        select:focus,
        textarea:focus {
            border-color: #990000;
            outline: none;
            box-shadow: 0 0 0 2px rgba(153, 0, 0, 0.2);
        }
        
        .size-options {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(110px, 1fr));
            gap: 15px;
            margin-top: 15px;
        }
        
        .size-option {
            display: flex;
            flex-direction: column;
            align-items: center;
            background: white;
            padding: 15px 10px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .size-option:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 10px rgba(0,0,0,0.15);
        }
        
        .size-option label {
            font-weight: bold;
            margin-bottom: 10px;
            color: #990000;
        }
        
        .size-option input {
            width: 70px;
            text-align: center;
            padding: 8px;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        
        .team-options {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 15px;
        }
        
        .team-option {
            border: 2px solid #ddd;
            border-radius: 8px;
            padding: 20px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s;
        }
        
        .team-option:hover {
            border-color: #990000;
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .team-option.selected {
            border-color: #990000;
            background-color: rgba(153, 0, 0, 0.05);
        }
        
        .team-option i {
            font-size: 40px;
            margin-bottom: 15px;
            display: block;
        }
        
        .team-option.boys i {
            color: #1a73e8;
        }
        
        .team-option.girls i {
            color: #e81a6d;
        }
        
        .team-option.both i {
            color: #990000;
        }
        
        .payment-options {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 15px;
        }
        
        .payment-option {
            border: 2px solid #ddd;
            border-radius: 8px;
            padding: 15px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s;
        }
        
        .payment-option:hover {
            border-color: #990000;
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        
        .payment-option.selected {
            border-color: #990000;
            background-color: rgba(153, 0, 0, 0.05);
        }
        
        .payment-option i {
            font-size: 40px;
            margin-bottom: 10px;
            display: block;
        }
        
        .payment-option.cashapp i {
            color: #00D632;
        }
        
        .payment-option.cash i {
            color: #28a745;
        }
        
        .payment-details {
            display: none;
            margin-top: 20px;
            padding: 15px;
            background-color: #f0f8ff;
            border-radius: 8px;
            border-left: 4px solid #2196F3;
        }
        
        .submit-btn {
            background: linear-gradient(135deg, #990000 0%, #770000 100%);
            color: white;
            border: none;
            padding: 16px 25px;
            font-size: 18px;
            border-radius: 8px;
            cursor: pointer;
            display: block;
            width: 100%;
            margin-top: 20px;
            font-weight: bold;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        
        .submit-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(153, 0, 0, 0.3);
        }
        
        .submit-btn:active {
            transform: translateY(0);
        }
        
        footer {
            text-align: center;
            padding: 20px;
            background-color: #1a1a1a;
            color: #ccc;
        }
        
        .contact-info {
            margin-top: 10px;
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            .size-options, .team-options, .payment-options {
                grid-template-columns: repeat(2, 1fr);
            }
            
            h1 {
                font-size: 2rem;
            }
            
            .form-content {
                padding: 20px;
            }
        }
        
        @media (max-width: 480px) {
            .size-options, .team-options, .payment-options {
                grid-template-columns: 1fr;
            }
            
            body {
                padding: 10px;
            }
            
            header {
                padding: 20px 15px;
            }
        }
        
        .confirmation {
            display: none;
            text-align: center;
            padding: 40px;
            background-color: #f9f9f9;
            border-radius: 8px;
            margin-top: 20px;
        }
        
        .confirmation i {
            font-size: 60px;
            color: #4CAF50;
            margin-bottom: 20px;
        }

        .price-display {
            text-align: center;
            font-size: 1.2rem;
            margin: 15px 0;
            padding: 10px;
            background-color: #f8f9fa;
            border-radius: 8px;
            font-weight: bold;
        }
        
        .price-display span {
            color: #990000;
        }
        
        .price-highlight {
            background-color: #990000;
            color: white;
            padding: 8px 15px;
            border-radius: 20px;
            font-weight: bold;
            margin-left: 10px;
            font-size: 1rem;
        }
        
        .email-notice {
            background-color: #e8f5e9;
            padding: 15px;
            border-radius: 8px;
            margin-top: 20px;
            border-left: 4px solid #4CAF50;
            font-size: 0.9rem;
        }
        
        .email-notice strong {
            color: #990000;
        }
        
        .email-highlight {
            background-color: #ffebee;
            padding: 10px;
            border-radius: 6px;
            margin: 10px 0;
            border-left: 4px solid #f44336;
        }
        
        .email-highlight p {
            margin: 5px 0;
            font-weight: bold;
        }
        
        .deadline {
            background-color: #e3f2fd;
            padding: 10px;
            border-radius: 6px;
            margin: 10px 0;
            border-left: 4px solid #2196f3;
        }
        
        .deadline p {
            margin: 5px 0;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="logo">
                <i class="fas fa-wrestling"></i>
            </div>
            <h1>Fountain Fort Carson Wrestling</h1>
            <p class="subtitle">Pre-order your <span class="team-name">Trojan Wrestling</span> shirts for the 2025-2026 season</p>
        </header>
        
        <div class="form-content">
            <div class="instructions">
                <h3><i class="fas fa-info-circle"></i> Important Information</h3>
                
                <div class="deadline">
                    <p><i class="fas fa-calendar-day"></i> <strong>Pre-orders close: November 24, 2025</strong></p>
                    <p><i class="fas fa-truck"></i> <strong>Shirts will be delivered in early December</strong></p>
                </div>
                
                <p>Thank you for supporting Trojan Wrestling! Please complete this form to pre-order your t-shirts.</p>
                <p><strong>T-shirt price: <span class="price-highlight">$25 each</span></strong></p>
                
                <div class="email-highlight">
                    <p><i class="fas fa-envelope"></i> <strong>ALL PRE-ORDERS WILL BE EMAILED TO:</strong></p>
                    <p>spenserstufflebeam@gmail.com</p>
                    <p>spenserjamesstufflebeam@gmail.com</p>
                    <p><strong>You will receive a confirmation email after submitting your order.</strong></p>
                </div>
                
                <div class="email-notice">
                    <p><strong>This form works on all devices:</strong></p>
                    <p>• Smartphones</p>
                    <p>• Tablets</p>
                    <p>• Laptops</p>
                    <p>• Desktop computers</p>
                </div>
            </div>
            
            <form id="preorder-form">
                <input type="hidden" id="form-action" name="form-action" value="">
                
                <div class="form-section">
                    <h2><i class="fas fa-users"></i> Team Selection</h2>
                    
                    <div class="form-group">
                        <label>Which team are you supporting?*</label>
                        <div class="team-options">
                            <div class="team-option boys" data-team="boys">
                                <i class="fas fa-male"></i>
                                <h3>Boys Team</h3>
                                <p>Support our Boys Wrestling Team</p>
                            </div>
                            <div class="team-option girls" data-team="girls">
                                <i class="fas fa-female"></i>
                                <h3>Girls Team</h3>
                                <p>Support our Girls Wrestling Team</p>
                            </div>
                            <div class="team-option both" data-team="both">
                                <i class="fas fa-people-group"></i>
                                <h3>Both Teams</h3>
                                <p>Support both Wrestling Teams</p>
                            </div>
                        </div>
                        <input type="hidden" id="team-selection" name="team-selection" required>
                    </div>
                </div>
                
                <div class="form-section">
                    <h2><i class="fas fa-user"></i> Your Information</h2>
                    
                    <div class="form-group">
                        <label for="name">Full Name*</label>
                        <input type="text" id="name" name="name" required placeholder="Enter your full name">
                    </div>
                    
                    <div class="form-group">
                        <label for="email">Email Address*</label>
                        <input type="email" id="email" name="email" required placeholder="Enter your email address">
                    </div>
                    
                    <div class="form-group">
                        <label for="phone">Phone Number*</label>
                        <input type="tel" id="phone" name="phone" required placeholder="Enter your phone number">
                    </div>
                    
                    <div class="form-group">
                        <label for="relationship">Relationship to Wrestler</label>
                        <select id="relationship" name="relationship">
                            <option value="">Select one</option>
                            <option value="parent">Parent</option>
                            <option value="sibling">Sibling</option>
                            <option value="relative">Relative</option>
                            <option value="friend">Friend</option>
                            <option value="community">Community Member</option>
                            <option value="other">Other</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <label for="wrestler">Wrestler You're Supporting (optional)</label>
                        <input type="text" id="wrestler" name="wrestler" placeholder="Enter wrestler's name">
                    </div>
                </div>
                
                <div class="form-section">
                    <h2><i class="fas fa-tshirt"></i> T-Shirt Selection</h2>
                    
                    <div class="form-group">
                        <label>Select sizes and quantities (<strong>$25 each</strong>):</label>
                        <div class="size-options">
                            <div class="size-option">
                                <label for="xs">XS</label>
                                <input type="number" id="xs" name="xs" min="0" value="0" class="shirt-qty">
                            </div>
                            <div class="size-option">
                                <label for="s">S</label>
                                <input type="number" id="s" name="s" min="0" value="0" class="shirt-qty">
                            </div>
                            <div class="size-option">
                                <label for="m">M</label>
                                <input type="number" id="m" name="m" min="0" value="0" class="shirt-qty">
                            </div>
                            <div class="size-option">
                                <label for="l">L</label>
                                <input type="number" id="l" name="l" min="0" value="0" class="shirt-qty">
                            </div>
                            <div class="size-option">
                                <label for="xl">XL</label>
                                <input type="number" id="xl" name="xl" min="0" value="0" class="shirt-qty">
                            </div>
                            <div class="size-option">
                                <label for="xxl">XXL</label>
                                <input type="number" id="xxl" name="xxl" min="0" value="0" class="shirt-qty">
                            </div>
                        </div>
                    </div>
                    
                    <div class="price-display">
                        Total: <span id="total-price">$0.00</span>
                    </div>
                    
                    <div class="form-group">
                        <label for="comments">Special Requests or Comments</label>
                        <textarea id="comments" name="comments" rows="3" placeholder="Any special instructions or requests"></textarea>
                    </div>
                </div>
                
                <div class="form-section">
                    <h2><i class="fas fa-money-bill-wave"></i> Payment Method</h2>
                    
                    <div class="form-group">
                        <label>Select your payment method:*</label>
                        <div class="payment-options">
                            <div class="payment-option cashapp" data-method="cashapp">
                                <i class="fab fa-bitcoin"></i>
                                <h3>Cash App</h3>
                                <p>Send to: $stufflebeam34</p>
                            </div>
                            <div class="payment-option cash" data-method="cash">
                                <i class="fas fa-money-bill"></i>
                                <h3>Cash</h3>
                                <p>Pay in person</p>
                            </div>
                        </div>
                        <input type="hidden" id="payment-method" name="payment-method" required>
                    </div>
                    
                    <div class="payment-details" id="cashapp-details">
                        <h3><i class="fab fa-bitcoin"></i> Cash App Instructions</h3>
                        <p>1. Open your Cash App</p>
                        <p>2. Send payment to: <strong>$stufflebeam34</strong></p>
                        <p>3. Include your name in the notes</p>
                        <p>4. Take a screenshot of your payment confirmation</p>
                    </div>
                    
                    <div class="payment-details" id="cash-details">
                        <h3><i class="fas fa-money-bill"></i> Cash Payment Instructions</h3>
                        <p>Please bring exact cash to the school office:</p>
                        <p><strong>Location:</strong> Fountain Fort Carson High School Office</p>
                        <p><strong>Hours:</strong> 7:30 AM - 3:30 PM, Monday-Friday</p>
                    </div>
                </div>
                
                <button type="submit" class="submit-btn">
                    <i class="fas fa-check-circle"></i> Submit Pre-Order
                </button>
            </form>
            
            <div class="confirmation" id="confirmation">
                <i class="fas fa-check-circle"></i>
                <h2>Thank You For Your Order!</h2>
                <p>Your pre-order has been received and emailed to:</p>
                <p><strong>spenserstufflebeam@gmail.com</strong></p>
                <p><strong>spenserjamesstufflebeam@gmail.com</strong></p>
                <p>Please complete your payment using your selected method.</p>
                <p><strong>Shirts will be delivered in early December</strong></p>
                <p>We'll contact you when the shirts are ready for pickup.</p>
                <p>Go Trojans!</p>
            </div>
        </div>
        
        <footer>
            <p>Fountain Fort Carson High School Wrestling</p>
            <p class="contact-info">For questions, contact Coach Spenser Stufflebeam: spenserstufflebeam@gmail.com or spenserjamesstufflebeam@gmail.com</p>
        </footer>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Calculate total price
            const pricePerShirt = 25;
            const quantityInputs = document.querySelectorAll('.shirt-qty');
            const totalDisplay = document.getElementById('total-price');
            
            function calculateTotal() {
                let total = 0;
                quantityInputs.forEach(input => {
                    total += parseInt(input.value) * pricePerShirt;
                });
                totalDisplay.textContent = `$${total.toFixed(2)}`;
            }
            
            quantityInputs.forEach(input => {
                input.addEventListener('input', calculateTotal);
            });
            
            // Team selection
            const teamOptions = document.querySelectorAll('.team-option');
            const teamSelectionInput = document.getElementById('team-selection');
            
            teamOptions.forEach(option => {
                option.addEventListener('click', function() {
                    // Remove selected class from all options
                    teamOptions.forEach(opt => opt.classList.remove('selected'));
                    
                    // Add selected class to clicked option
                    this.classList.add('selected');
                    
                    // Set the team selection value
                    const team = this.getAttribute('data-team');
                    teamSelectionInput.value = team;
                });
            });
            
            // Payment method selection
            const paymentOptions = document.querySelectorAll('.payment-option');
            const paymentMethodInput = document.getElementById('payment-method');
            const paymentDetails = document.querySelectorAll('.payment-details');
            
            paymentOptions.forEach(option => {
                option.addEventListener('click', function() {
                    // Remove selected class from all options
                    paymentOptions.forEach(opt => opt.classList.remove('selected'));
                    
                    // Add selected class to clicked option
                    this.classList.add('selected');
                    
                    // Set the payment method value
                    const method = this.getAttribute('data-method');
                    paymentMethodInput.value = method;
                    
                    // Hide all payment details
                    paymentDetails.forEach(detail => {
                        detail.style.display = 'none';
                    });
                    
                    // Show selected payment details
                    document.getElementById(`${method}-details`).style.display = 'block';
                });
            });
            
            // Form validation and submission
            document.getElementById('preorder-form').addEventListener('submit', function(e) {
                e.preventDefault();
                
                // Basic validation
                const name = document.getElementById('name').value;
                const email = document.getElementById('email').value;
                const phone = document.getElementById('phone').value;
                const teamSelection = teamSelectionInput.value;
                const paymentMethod = paymentMethodInput.value;
                
                if (!name || !email || !phone) {
                    alert('Please fill in all required fields (name, email, phone)');
                    return;
                }
                
                if (!teamSelection) {
                    alert('Please select which team you are supporting');
                    return;
                }
                
                if (!paymentMethod) {
                    alert('Please select a payment method');
                    return;
                }
                
                // Check if at least one shirt was ordered
                const quantities = [
                    parseInt(document.getElementById('xs').value),
                    parseInt(document.getElementById('s').value),
                    parseInt(document.getElementById('m').value),
                    parseInt(document.getElementById('l').value),
                    parseInt(document.getElementById('xl').value),
                    parseInt(document.getElementById('xxl').value)
                ];
                
                const totalOrdered = quantities.reduce((total, qty) => total + qty, 0);
                
                if (totalOrdered === 0) {
                    alert('Please order at least one t-shirt');
                    return;
                }
                
                // Set the form action to send to both email addresses
                const form = document.getElementById('preorder-form');
                form.action = 'https://formsubmit.co/spenserstufflebeam@gmail.com';
                
                // Add CC as a hidden field for the second email
                const ccInput = document.createElement('input');
                ccInput.type = 'hidden';
                ccInput.name = '_cc';
                ccInput.value = 'spenserjamesstufflebeam@gmail.com';
                form.appendChild(ccInput);
                
                // Add formsubmit configuration
                const subjectInput = document.createElement('input');
                subjectInput.type = 'hidden';
                subjectInput.name = '_subject';
                subjectInput.value = `New ${teamSelection.charAt(0).toUpperCase() + teamSelection.slice(1)} Team T-Shirt Pre-Order`;
                form.appendChild(subjectInput);
                
                const templateInput = document.createElement('input');
                templateInput.type = 'hidden';
                templateInput.name = '_template';
                templateInput.value = 'table';
                form.appendChild(templateInput);
                
                const nextInput = document.createElement('input');
                nextInput.type = 'hidden';
                nextInput.name = '_next';
                nextInput.value = '#confirmation';
                form.appendChild(nextInput);
                
                const captchaInput = document.createElement('input');
                captchaInput.type = 'hidden';
                captchaInput.name = '_captcha';
                captchaInput.value = 'false';
                form.appendChild(captchaInput);
                
                // Submit the form
                form.submit();
                
                // Show confirmation message
                document.getElementById('preorder-form').style.display = 'none';
                document.getElementById('confirmation').style.display = 'block';
            });
        });
    </script>
</body>
</html>
