Sales Return Automation & Validation – Custom Function
---
This custom function validates and processes sales returns by comparing refunded items against the corresponding sales order, ensuring sufficient quantities are available for return. It handles validation failures by generating clear, actionable error messages for any discrepancies. Upon successful processing, it constructs and sends an HTML email notification summarizing the sales return details, including any failed or skipped items.

Custome function Mappings:
---

Output Variable Name : validationwithMutipleSKU_3

    organization_id: ${fetchSalesOrder_6.organization_id}
    salesorder_id: ${fetchSalesOrder_6.salesorder_id}
    order_id: ${fetchSalesOrder_6.salesorder_number}
    refund_line_items: ${trigger.refund_line_items}
    refund_line_items: ${fetchSalesOrder_6.line_items}
