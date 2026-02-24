OEM orderings systems = B2B brand portals
dealership DMS systemts = DLsoftwarfe

Question to chatGPT:

When a authorized motorcycle dealership uses a OEM portal from a motorcycle brand and orders a bike through pre-order. How does that look like? Because apparently the dealership doesn't see the VIN number from the OEM portals, only information like chassi, model and color of the bike. Therefore they usually have to create a temporary product with a product number in DLsoftware.

----------
Great question — this is a **very common operational gap** between OEM ordering systems and dealership DMS systems like DLsoftware.

I’ll break this down clearly from a real dealership workflow perspective.

---
# 1. What Happens in the OEM Portal (Pre-Order Stage)

When an authorized dealer orders a motorcycle through an OEM portal (for example from brands like Yamaha Motor Company, Kawasaki Heavy Industries, BMW Motorrad, or Honda Motor Co.), the process usually looks like this:

### In the OEM Portal the dealer sees:

- Model (e.g., MT-07, Ninja 650, R 1250 GS)
    
- Color / color code
    
- Model year
    
- Variant / trim
    
- Production status
    
- Estimated delivery window
    
- Order reference number
    
- Sometimes engine number (rare)
    
- **Usually NOT the VIN at pre-order stage**
    

👉 The VIN is typically generated:

- After production is scheduled
    
- Or once the unit leaves the factory
    
- Or sometimes only once it reaches the national distributor
    

So at pre-order stage, the bike is basically:

> “Allocation slot for X model in Y color”

Not yet a specific physical unit.

---
# 2. Why VIN Is Not Visible Yet

The VIN is assigned when:

1. The bike enters production
    
2. Or production is completed
    
3. Or it is released to logistics
    

Until then, the OEM system only reserves:

- Model
    
- Spec
    
- Production capacity slot
    

So from a systems perspective:

- The OEM system is production-driven
    
- The DMS (like DLsoftware) is VIN-driven
    

That’s the root of the mismatch.

---
# 3. How This Looks in DLsoftware (Dealer Side)

Because DLsoftware requires inventory items to:

- Be sellable
    
- Be reservable
    
- Be financeable
    
- Be part of stock valuation
    

But no VIN exists yet…

👉 The dealership typically creates a **temporary inventory unit**.

### Typical workaround in DLsoftware:

They create:

- Product number: e.g. `TEMP-MT07-BLUE-01`
    
- Description: “MT-07 2025 Blue – Preorder”
    
- No VIN
    
- Chassis field empty or filled with placeholder like:
    
    - `PREORDER`
        
    - `TBA`
        
    - `000000000`
        

This temporary product allows:

- Sales contract creation
    
- Deposit invoice
    
- Reservation to customer
    
- Sales pipeline tracking
    
- Commission registration
    
- Financing pre-approval

---
# 4. When the VIN Finally Arrives

Later — when the distributor updates the portal — the dealer finally sees:

- VIN
    
- Final invoice
    
- Shipping confirmation
    

Now the dealership must:

### Either:

**Option A (Best Practice):**

- Convert the temporary unit
    
- Update VIN field
    
- Update cost price
    
- Link OEM invoice
    
- Change stock status from “ordered” to “in stock”
    

**Option B (Messier Reality in Many Dealerships):**

- Create a new inventory item with VIN
    
- Transfer deposit manually
    
- Close temporary product
    
- Adjust accounting entries
    

Option B creates accounting noise.

---
# 5. Why This Is Operationally Risky

Because during preorder stage:

- No VIN = no legal vehicle
    
- No VIN = cannot register
    
- No VIN = cannot insure
    
- No VIN = financing banks may hesitate
    

So the DMS entry is more of a “financial placeholder” than a physical unit.

This causes:

- Stock report inconsistencies
    
- Margin forecasting errors
    
- Double entries
    
- Confusion between sales & accounting

---
# 6. What a Clean Integrated Flow Would Look Like (Ideal Scenario)

If DLsoftware were fully integrated with the OEM API:

1. Dealer places order in OEM portal
    
2. Pre-order is automatically pushed to DLsoftware as:
    
    - “Incoming unit – no VIN”
        
    - Linked to OEM order ID
        
3. When VIN is assigned:
    
    - The record auto-updates
        
    - Cost invoice auto-matches
        
    - Status changes to “in transit”
        

But most OEMs don’t expose real-time VIN APIs to DMS providers.

---
# 7. Why OEMs Structure It This Way

Motorcycle production is often:

- Batch-based
    
- Allocation-controlled
    
- Regionally distributed
    

Dealers don’t order specific VINs.  
They order:

> Production slots.

VIN assignment happens later in the supply chain.

---
# 8. What This Means for Sales Workflow

In real dealership life:

Salesperson:

- Sells “a MT-07 in blue”
    
- Takes deposit
    
- Promises estimated delivery
    

Accounting:

- Books deposit to temporary unit
    

Stock manager:

- Waits for VIN update
    

Admin:

- Later matches VIN to customer contract
    

It’s operationally fragmented unless processes are very disciplined.

---
# 9. Practical Tip for DLsoftware Users

The cleanest internal workflow is:

✔ Create a dedicated “Pre-Order Inventory Type”  
✔ Use structured temporary product numbers  
✔ Never duplicate unit records  
✔ Update VIN directly on existing item  
✔ Lock editing rights to prevent double creation