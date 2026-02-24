
Question to chatGPT:

hey chat, you're an expert on the motorcycle business and knows everything about DLsoftware. In my company we have sales personel using pre-orders in the OEM portals when they order motorcyces. While the Administrator / Accountant person using purchase orders when ordering motorcycles. As I know the purchase order is more a financial commitment document. Is there a benificial reason to use pre-orders as the way to order bikes or is it mostly done of convenience? because I know that I creates problems when localizing goods in the DLsoftware system.

---
Great question — this is a **very common operational tension** in motorcycle dealerships using DLSoftware (especially in powersports with OEM portal integrations).

You’re thinking about this correctly:  
A **Purchase Order (PO)** is a financial commitment document.  
A **Pre-Order** is typically an inventory pipeline / reservation tool.

Let’s break this down strategically.

---

# 1️⃣ What a Purchase Order Does (Financial Perspective)

Inside dealership systems like **DLSoftware**, a **PO**:

- Creates a formal financial liability
    
- Impacts committed inventory
    
- Feeds into:
    
    - Floorplan tracking
        
    - Open AP reporting
        
    - Cash flow forecasting
        
    - Inventory aging reports
        
- Creates a clean receiving process
    
- Allows proper cost allocation (freight, setup, PDI, surcharges)
    

From an accounting standpoint — this is the cleanest and most controlled workflow.

This is why your accountant prefers it.

---

# 2️⃣ What a Pre-Order Does (Sales Perspective)

In OEM portals (e.g., allocation systems from manufacturers like:

- Honda Motor Co.
    
- Yamaha Motor Company
    
- KTM AG
    
- Harley-Davidson
    

Salespeople often use **Pre-Orders** because:

- They’re fast
    
- They match OEM allocation terminology
    
- They reserve units against customer deposits
    
- They feel like a “soft commitment”
    
- They don’t require cost finalization at time of order
    
- They’re easier operationally from the showroom
    

It’s often convenience + workflow habit.

---

# 3️⃣ Why Pre-Orders Create Problems in DLSoftware

You already identified the core issue: **localization**.

Here’s what typically breaks:

### ❌ Inventory localization mismatches

- The unit arrives
    
- It’s not tied to a formal PO
    
- Receiving becomes manual
    
- Costs get adjusted after the fact
    

### ❌ Cost control problems

- Freight & surcharges are added late
    
- Floorplan interest start date gets unclear
    
- Margin reports become distorted
    

### ❌ Reporting inconsistencies

- Open order reports don’t match accounting
    
- Inventory aging can start from wrong dates
    
- Deposit-to-unit matching gets messy
    

### ❌ Internal control weakness

Pre-orders are not strong financial control documents.

For administrators, that’s a red flag.

---

# 4️⃣ Is There a Strategic Advantage to Using Pre-Orders?

Yes — but only in specific cases.

### ✅ When Pre-Orders Make Sense

**1. Allocation-Based Ordering**  
If the OEM system forces allocation submissions before final confirmation.

**2. Customer-Specific Factory Orders**  
If the unit is sold before it exists, and:

- MSRP may change
    
- Freight may vary
    
- Incentives aren’t confirmed
    

**3. Sales-Controlled Pipeline Visibility**  
Sales managers like to see pipeline units separate from stock inventory.

---

# 5️⃣ But Should Pre-Orders Replace POs?

From a dealership operations standpoint:

**No — not as the primary ordering method.**

Best practice in high-performing dealerships:

> Pre-Order in OEM Portal → Immediately Generate Purchase Order in DLSoftware

That gives you:

- Sales flexibility
    
- Accounting control
    
- Clean receiving
    
- Proper cost structure
    
- Accurate margin reporting
    

---

# 6️⃣ Why DLSoftware Struggles With Pre-Orders Alone

DLSoftware is built around:

- Inventory lifecycle tracking
    
- GL integration
    
- Floorplan liability management
    
- Accurate receiving and costing
    

It expects:

> Order → Receive → Localize → Cost → Sell

When Pre-Orders bypass the PO step, the lifecycle breaks.

That’s why localization becomes messy.

---

# 7️⃣ What I Recommend (Operationally)

If you want alignment between Sales and Accounting:

### 🔹 Option 1 – Hybrid Control Model (Best Practice)

- Sales enters Pre-Order in OEM
    
- Admin creates matching PO in DLSoftware same day
    
- Unit is received against PO
    
- Pre-Order is linked to customer deposit
    

Clean. Controlled. Scalable.

---

### 🔹 Option 2 – Administrator-Controlled Ordering

Sales submits order request internally.  
Admin places OEM order + creates PO simultaneously.

More control, slightly slower.

---

# 8️⃣ The Real Question: What Type of Dealership Are You?

Let me personalize this to you:

If you're:

- Multi-line dealer
    
- Carrying floorplan
    
- Tracking departmental profitability
    
- Growing inventory volume
    

Then **Purchase Orders must be your backbone.**

If you're:

- Small volume
    
- Mostly pre-sold units
    
- Low floorplan exposure
    

Then pre-orders might feel easier.

---

# Bottom Line

Pre-orders are mostly:

- Convenience
    
- Sales-driven workflow
    
- OEM terminology influence
    

Purchase Orders are:

- Financial discipline
    
- Inventory accuracy
    
- Reporting integrity
    
- Scalable operations
    

If localization problems are happening, that’s a symptom — not the disease.

The root issue is:

> Sales workflow is bypassing financial structure.


---
Another ChatGPT question:

Thanks! since the sales people don't order motorcycles through purchase order, the admin gets an invoice without a purchase number. this makes it complicated to find whom the vehicle belongs to in the system. Is this because they're using pre-order?

---

Yes — **this is happening because they’re using Pre-Orders instead of Purchase Orders.**

What you’re describing is a classic breakdown between **sales pipeline control** and **accounting control** in DLSoftware.

Let’s walk through exactly why this happens.

---

# What’s Actually Causing the Problem

When sales uses a **Pre-Order in the OEM portal** (for example with Honda Motor Co. or Yamaha Motor Company):

- The OEM confirms the order
    
- The bike ships
    
- The OEM sends an invoice
    
- The invoice references:
    
    - Model
        
    - VIN
        
    - Maybe dealer number
        
    - **But not your internal DLSoftware PO number**
        

Because…

👉 No Purchase Order was created in DLSoftware.

So when Admin receives the invoice:

- There’s no matching PO in the system
    
- No receiving document
    
- No committed inventory record
    
- No financial liability pre-created
    

Now the admin must:

- Manually search by VIN
    
- Ask sales who ordered it
    
- Dig through deposits
    
- Check pre-orders
    
- Guess which customer it belongs to
    

That’s the friction you're feeling.

---

# Why This Doesn’t Happen With Purchase Orders

When a PO exists in DLSoftware:

1. The unit is already expected in the system
    
2. It is tied to:
    
    - A salesperson (if entered properly)
        
    - A customer (if pre-sold)
        
    - A cost estimate
        
3. When the invoice arrives:
    
    - Admin receives against PO
        
    - Costs match
        
    - Localization is automatic
        
    - Ownership trail is clean
        

The PO acts as a **bridge between Sales and Accounting**.

Without it, the bridge doesn’t exist.

---

# The Core Structural Issue

Pre-Orders are:

- Sales workflow tools
    
- Reservation tools
    
- Allocation tools
    

They are **not accounting documents**.

DLSoftware is built around:

> Financial document → Receiving → Inventory → Sale

Pre-Orders skip step one.

That’s why you're experiencing:

- Invoice confusion
    
- VIN hunting
    
- Ownership uncertainty
    
- Localization complications
    
- Cost allocation errors
    

---

# Why Sales Likes Pre-Orders

From their perspective:

- It feels faster
    
- It mirrors OEM language
    
- It reserves units for customers
    
- It avoids waiting for admin
    

But they’re unknowingly creating downstream accounting chaos.

---

# The Exact Reason You Can’t Find Who the Vehicle Belongs To

Because:

- The Pre-Order lives in Sales space
    
- The Invoice lives in Accounting space
    
- There is no system document connecting the two
    

The PO is that connector.

Without it, you’re manually reconstructing intent after the fact.

---

# The Operational Risk (Beyond Annoyance)

This doesn’t just create inconvenience — it can cause:

- Margin distortions
    
- Units sold before properly received
    
- Floorplan interest miscalculations
    
- Deposit misapplication
    
- Duplicate units in system
    
- Audit trail weakness
    

In larger dealerships, this becomes very expensive very quickly.

---

# The Clean Fix

Best practice workflow:

1. Sales submits OEM Pre-Order
    
2. Same day, Admin creates matching PO in DLSoftware
    
3. PO number is documented internally
    
4. When invoice arrives → Receive against PO
    
5. VIN auto-links to correct customer / salesperson
    

Now:

- Invoice matches system
    
- Unit is traceable
    
- Localization is clean
    
- Accountability is clear
    

---

# Direct Answer to Your Question

> Is this because they’re using Pre-Orders?

Yes.

More precisely:  
It’s because **Pre-Orders are being used without a corresponding Purchase Order in DLSoftware.**

That’s the structural flaw.


---
Another chatGPT Question:

Okay thanks! So you say the purchase order is created in the DLsoftware? because I got the feeling that you could make a purchase order inside the OEM portal?

One other thing I want to know about is that when the sales department has made a pre-order on the motorcycle, they have to create a temporary product with a product id in DLsoftware because there's no VIN number on the bike yet. when there's a VIN number on bike, the swedish transport agency can register the vehicle. once the MC is registered, the temporary product is replaced with the real product. Is the temporary product a type of 'model product'? And those this happen because of the pre-order vs. purchase order operational tension?

---
Excellent — now we’re getting into the real structural mechanics of how this is set up.

You’re asking exactly the right questions.

---

# 1️⃣ Can You Create a Purchase Order in the OEM Portal?

Short answer:

**No — not in the way DLSoftware needs it.**

When you “create a PO” inside an OEM portal (for example with Honda Motor Co. or Yamaha Motor Company):

- You are creating an **order confirmation**
    
- Or an **allocation request**
    
- Or a **factory order**
    

That document exists in the OEM’s system.

It does **not**:

- Create a liability in your accounting
    
- Create committed inventory in DLSoftware
    
- Generate a receivable / payable structure in your books
    

DLSoftware needs its **own internal Purchase Order** because it drives:

- Inventory pipeline
    
- Cost expectation
    
- GL integration
    
- Receiving process
    
- VIN matching
    

So yes — the PO I’m referring to is created inside DLSoftware.

The OEM portal cannot replace that function.

---

# 2️⃣ About the “Temporary Product” Before VIN Exists

Now this is very interesting — and very common in Scandinavian dealerships.

You described:

1. Sales makes a pre-order
    
2. No VIN exists yet
    
3. They create a temporary product ID in DLSoftware
    
4. Once VIN is assigned and registered at Swedish Transport Agency
    
5. The temporary product is replaced with the real VIN product
    

Let’s break this down.

---

# 3️⃣ Is the Temporary Product a “Model Product”?

Yes — structurally speaking.

It’s acting as:

- A model-level placeholder
    
- A non-serialized inventory item
    
- A pipeline representation of a future serialized unit
    

It represents:

> “We expect one Yamaha MT-09, but we don’t yet know which VIN.”

So conceptually it is a **model product placeholder**.

But operationally?

It’s a workaround.

---

# 4️⃣ Why This Is Happening

This workflow usually appears when:

- Pre-orders are used
    
- No DLSoftware PO is created
    
- No VIN exists
    
- Sales wants to:
    
    - Take deposit
        
    - Create order contract
        
    - Secure customer deal
        

Since DLSoftware inventory is VIN-based (serialized inventory), it expects:

> VIN → Inventory → Sale

But sales wants:

> Customer → Contract → Future Bike

So they create a fake product to bridge the gap.

---

# 5️⃣ Does This Happen Because of Pre-Order vs PO Tension?

Indirectly — yes.

Here’s why:

If a **Purchase Order exists in DLSoftware**, you can:

- Create a “unit on order” record
    
- Tie it to:
    
    - Model
        
    - Expected cost
        
    - Expected arrival
        
    - Salesperson
        
    - Customer (if pre-sold)
        

Even without VIN.

When VIN arrives:

- You update the PO line
    
- Receive against it
    
- Convert it into serialized inventory
    
- No fake product needed
    

The temporary product workaround usually appears when:

> Sales process outruns inventory process.

It’s not caused by pre-orders alone —  
It’s caused by lack of structured inventory pipeline management.

---

# 6️⃣ The Real Root Issue

Your dealership currently has:

### Sales System Logic:

“We sell future motorcycles.”

### DLSoftware Logic:

“We sell serialized inventory.”

Those two logics are not aligned.

So the temporary product is a bridge between:

- Future expectation
    
- Serialized accounting reality
    

---

# 7️⃣ The Swedish Registration Factor

In Sweden, VIN becomes critical because:

- Registration with Swedish Transport Agency requires it
    
- Insurance requires it
    
- Road legality requires it
    
- Financing often requires it
    

So you cannot finalize delivery without VIN.

That increases the pressure to create placeholders early.

---

# 8️⃣ Is This Dangerous?

It depends on volume.

At low volume:

- Annoying but manageable.
    

At higher volume:

- Margin distortion risk
    
- Double inventory risk
    
- Lost VIN linkage risk
    
- Cost allocation problems
    
- Audit trail weakness
    
- Deposit mismatches
    

And if someone forgets to replace the temporary product correctly?

You can distort gross profit reporting.

---

# 9️⃣ What a Structured System Would Look Like

Instead of temporary products:

1. Create DLSoftware Purchase Order (model-level, no VIN yet)
    
2. Mark as:
    
    - “Customer ordered”
        
    - Attach deposit
        
3. When VIN assigned:
    
    - Update PO
        
    - Receive serialized unit
        
4. Close temporary model line automatically
    

No fake SKU required.

---

# 1️⃣0️⃣ Bottom Line

Yes:

- The temporary product behaves like a model product.
    

And yes:

- It exists largely because your dealership is compensating for a structural gap between Pre-Orders and Purchase Orders.
    

But the deeper issue is:

> Your sales workflow is future-based.  
> Your inventory system is VIN-based.  
> There is no formal bridge document (PO) connecting them early enough.

---
Another chatGPT question:

Okay thanks! here's one thing I don't really get: you said that a purchase order is: "A formal document a buyer sends to a supplier saying > “I officially commit to buying this product at this price.”. Since it's made in the DLsoftware after you've made a pre-order on the bike, isn't it just the same as a purchase list? what is the difference there?

---
That’s a very sharp question — and this is where many dealerships get conceptually confused.

You’re absolutely right to challenge it.

Let’s separate **three different things** clearly:

1. OEM Order (Pre-Order in portal)
    
2. Purchase List (internal planning list)
    
3. Purchase Order (financial document in DLSoftware)
    

They look similar.  
They are not the same.

---

# 1️⃣ OEM Pre-Order (Portal Order)

When sales orders via the OEM portal (e.g. Honda Motor Co. or Yamaha Motor Company):

You are telling the manufacturer:

> “Ship us this model.”

That creates:

- A production/allocation instruction
    
- A future shipment
    
- An eventual invoice
    

But it does **not** create:

- A liability in your accounting
    
- A committed inventory record in DLSoftware
    
- A GL impact
    

It exists only in the OEM’s world.

---

# 2️⃣ Purchase List (Planning Tool)

A purchase list is basically:

> “Here are bikes we intend to order.”

It’s informational.  
It’s internal.  
It has no accounting weight.

You can delete it.  
You can change it.  
It doesn’t affect financial reports.

It’s a management tool.

---

# 3️⃣ Purchase Order in DLSoftware (This Is the Key Difference)

Even if it’s created _after_ the OEM pre-order, it is not “just a list.”

A Purchase Order inside DLSoftware:

- Creates expected inventory
    
- Creates committed cost
    
- Appears in open PO reports
    
- Bridges to Accounts Payable
    
- Structures the receiving process
    
- Can be audited
    
- Can’t just be casually deleted without trace
    

It is a **controlled financial document**, not a note.

---

# Why It’s Still a “Formal Commitment” Even If Created After the OEM Order

You might think:

> “If we already ordered from the OEM, then the PO in DLSoftware is just paperwork.”

Operationally, yes — the commercial commitment was made in the OEM portal.

But financially, the commitment has not yet been structured in your accounting system.

The PO in DLSoftware is not committing to the OEM.

It is committing your dealership’s accounting system to:

- Expect this liability
    
- Reserve this cost
    
- Prepare to receive this asset
    
- Track this inventory pipeline
    

It formalizes the transaction internally.

---

# Think of It Like This

OEM Pre-Order:

> Commitment between you and manufacturer.

DLSoftware Purchase Order:

> Commitment between sales and accounting.

That’s the structural difference.

---

# Why This Matters Practically

Without PO in DLSoftware:

When invoice arrives:

- No matching document
    
- No expected cost
    
- No assigned responsibility
    
- No structured receiving
    

With PO:

Invoice → Match to PO → Receive → Localize → Cost finalized → Clean margin.

It’s a control mechanism.

---

# The Core Difference in One Sentence

A purchase list says:

> “We plan to buy this.”

A purchase order in DLSoftware says:

> “Finance, prepare for this liability. Inventory, prepare to receive this asset.”

That’s the difference.

---

# Why Growing Dealerships Can’t Skip This

At 5 bikes/month?  
You can survive without structured POs.

At 30+ bikes/month?  
Things start breaking:

- Missed cost allocations
    
- Floorplan confusion
    
- Margin distortions
    
- Deposit misalignment
    
- Audit risk
    

The PO becomes your backbone.