# LabHomework6
Improve the following codes to implement SOLID principles in OOP.


<pre>public interface Order {

  void calculateTotal(double price, int quantity);

  void placeOrder(String customerName, String address);

  void generateInvoice(String fileName);
  
  void sendEmailNotification(String email);
}

public class OrderAction implements Order {

  @Override
  public void calculateTotal(double price, int quantity) {
    double total = price * quantity;
    System.out.println("Order total: $" + total);
  }

  @Override
  public void placeOrder(String customerName, String address) {
    // Simulate placing order in a system
    System.out.println("Order placed for " + customerName + " at " + address);
  }

  @Override
  public void generateInvoice(String fileName) {
    // Simulate generating invoice file
    System.out.println("Invoice generated: " + fileName);
  }

  @Override
  public void sendEmailNotification(String email) {
    // Simulate sending email notification
    System.out.println("Email notification sent to: " + email);
  }
}

public class OrderTest {

  public static void main(String[] args) {
    Order order = new OrderAction();
    order.calculateTotal(10.0, 2);
    order.placeOrder("John Doe", "123 Main St");

    // These methods might not be needed for all orders
    order.generateInvoice("order_123.pdf");
    order.sendEmailNotification("johndoe@example.com");
  }
}</pre>


![UML_Diagram_LabHW6](https://github.com/JuanCyriljosh/LabHomework6/assets/152839993/b9e1b31d-e934-4a02-8d60-c6905a2005d5)


