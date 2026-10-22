    **Sheet**	           **Column**	                **Description**
Sales_Transactions	        Order_ID	                Order identifier; raw sheet contains deliberate exact duplicates.
Sales_Transactions	        Order_Date	                Date the order was created.
Sales_Transactions	        Customer_ID	                Key to Customer_Master.
Sales_Transactions	        Product_ID	                Key to Product_Master.
Sales_Transactions	        Salesperson_ID	            Key to Salesperson_Master.
Sales_Transactions	        Region_Recorded	            Operationally typed region; may contain variants, blanks, or mismatch.
Sales_Transactions	        Channel_Raw	                Unstandardised sales channel.
Sales_Transactions	        Quantity	                Units sold; a few zero values are deliberate quality issu   es.
Sales_Transactions	        Discount_Pct	           Decimal discount, e.g. 0.10 = 10%.
Sales_Transactions	        Payment_Mode	               Customer payment method.
Sales_Transactions	        Delivery_Days	             Days from order to delivery; blank for cancelled orders.
Sales_Transactions	        Customer_Rating	             Rating from 1 to 5; some values are blank.
Sales_Transactions	        Order_Status	             Raw status text with case/spacing/spelling variants.
Product_Master	            Unit_Price	                 Standard selling price per unit in INR.
Product_Master	            Unit_Cost	                 Standard cost per unit in INR.
Customer_Master	            Region	                     Canonical customer region to use in reporting.
Monthly_Targets	            Month	                     First day of the target month.
Monthly_Targets	            Revenue_Target	             Monthly net-sales target by salesperson in INR.
Returns	                    Return_Qty	                 Units returned for an order.
Returns	                    Return_Status	             Operational stage of the return record.
