# Notes-Elite (Markdown Drill-Down)

> Tick as you go. Your app can also parse the HTML comments as **rules** to auto-add arse-covers into the Depot Notes summary.

---

## 0) Working at heights
- [ ] Ladder access required
- [ ] Scaffold tower – standard
- [ ] Scaffold tower – bridging
- [ ] Cantilever scaffold
- [ ] MEWP required
- [ ] Loft access: boarded
- [ ] Loft access: unboarded
- [ ] Flat roof: specialist builder to make good
- [ ] Ladder angle ~1:4 (≈75°); ~250 mm out per metre rise
- [ ] Max ladder reach ≈6 m; >2 storeys or >45° roof → scaffold
- [ ] Fixed loft ladder & permanent lighting required

---

## 1) Old boiler type → choose new system

### A) Old: Regular (open-vented with F&E)
#### Choose one
- [ ] **Stay Regular (open-vented)**
  - **Cylinder**
    - [ ] Keep existing open-vented cylinder
    - [ ] Replace open-vented cylinder
  - **Water services**
    - [ ] Hot from cylinder (gravity/pumped as existing)
    - [ ] Cold outlets continue from CWS where present
  - **Safety discharge**
    - [ ] Boiler PRV → outside, visible termination
  - **Condensate**
    - [ ] Internal trapped waste
    - [ ] External 42 mm insulated / soakaway / soil stack / pump if needed
  - **Gas**
    - [ ] Size for CH load; ≤1 mbar drop under load (calc)
  - **Flush / Filter / Radiators**
    - [ ] Clean (powerflush or chemical + inhibit)
    - [ ] Magnetic filter
    - [ ] TRVs & balance
  - **Controls**
    - [ ] Retain Y-plan / S-plan
    - [ ] Programmer/room stat / Hive compatible

- [ ] **Convert to System + Unvented**
  - **Cylinder (unvented)**
    - [ ] Size (L), coil, reheat
    - [ ] 16 A spur if required
    - [ ] Tundish + D2 safe termination (G3)
  - **Water**
    - [ ] All hot at mains pressure
    - [ ] Balanced cold to outlets / PRV where needed
  - **Safety discharge**
    - [ ] Cylinder T&P via tundish; Boiler PRV → outside
  - **Condensate / Gas / Flush / Controls** — as per sections below
  <!-- rule: open_to_sealed = true -->

- [ ] **Convert to Combi**
  - **Water (critical)**
    - [ ] Mains dynamic pressure ≥1.5–2.0 bar
    - [ ] Mains flow ≥12–14 l/min (match combi spec)
    - [ ] Remove cylinder, CWS & F&E
    - [ ] Remove any shower pumps/power showers
  - **Safety discharge**
    - [ ] Boiler PRV → outside, visible termination
  - **Condensate**
    - [ ] Internal trap OR external 42 mm insulated / soakaway / soil stack / pump
  - **Gas**
    - [ ] Size for full DHW input; confirm meter (U6≈63 kW)
    - [ ] Target ≤1 mbar drop at max DHW load
  - **Flush / Filter / Radiators**
    - [ ] Clean; magnetic filter; TRVs; balance
  - **Controls**
    - [ ] Simple stat / load comp / Hive Mini
  <!-- rule: open_to_sealed = true -->
  <!-- rule: combi_selected = true -->

---

### B) Old: System boiler (with cylinder)
#### Old cylinder type
- [ ] Open-vented cylinder (with CWS/F&E)
- [ ] Unvented cylinder (G3)
- [ ] Thermal store / storage combi

#### Choose new system
- [ ] **Stay System + Unvented** (or replace unvented/Mixergy)
  - Follow **Unvented** steps (tundish/D2, G3, 16 A if req)
  <!-- rule: unvented_selected = true -->
- [ ] **Convert to Combi**
  - Remove cylinder/CWS; verify mains; resize gas for DHW
  <!-- rule: combi_selected = true -->
- [ ] **Convert to Regular (open-vented)**
  - Reinstate CWS & F&E; confirm vent & feed routes

---

### C) Old: Combi (existing)
- [ ] **Combi → Combi (swap)**
  - Verify mains flow/pressure match DHW spec
  - PRV/condensate/gas/flush/filter as below
  <!-- rule: combi_selected = true -->
- [ ] **Combi → System + Unvented**
  - Add G3 cylinder with tundish/D2; combi becomes system boiler (CH only)
  <!-- rule: unvented_selected = true -->
- [ ] **Combi → Regular (open-vented)**
  - Reintroduce CWS & F&E; Y/S-plan & wiring centre

---

### D) Old: Thermal store / Storage combi
- [ ] → **Combi (instant DHW)** — remove store; confirm mains; gas upsizing likely
  <!-- rule: combi_selected = true -->
- [ ] → **System + Unvented** — specify cylinder, discharge route, electrics
  <!-- rule: unvented_selected = true -->
- [ ] → **Regular (open-vented)** — reinstate CWS/F&E

---

### E) Old: Warm air / None
- [ ] → **Combi + radiators** (full wet system)
  <!-- rule: combi_selected = true -->
- [ ] → **System + Unvented + radiators**
  <!-- rule: unvented_selected = true -->
- [ ] → **Regular (open-vented) + radiators**

---

## 2) Universal requirements (tick for all installs)

### 2.1 Water services
- [ ] Measure mains **static**/**dynamic** pressure and **flow (l/min)**
- [ ] PRV/strainer/scale control as required
- [ ] Stop tap/service valve accessible
- [ ] Secondary return present? (integrate or isolate)

### 2.2 Safety discharges
- [ ] **Boiler PRV** → outside, visible & safe termination
- [ ] **Cylinder T&P (unvented only)** → tundish + D2 to safe termination (G3)
  <!-- rule: unvented_selected = true -->

### 2.3 Condensate (all condensing boilers)
- [ ] Internal: trapped waste
- [ ] External: **42 mm** insulated, correct fall; **soakaway** or **soil stack**
- [ ] Pump if gravity route unfeasible; neutraliser if MI requires
  <!-- rule: condensate_present = true -->

### 2.4 Gas (calculate, don’t guess)
- [ ] Meter type/capacity confirmed (U6≈63 kW, U16≈169 kW aggregate)
- [ ] Pipe-sizing calcs; target **≤1 mbar** drop at appliance under full load
- [ ] Minimise bends; upsize sections (e.g., 28 mm) where needed
  <!-- rule: gas_checked = true -->

---

## 3) System hygiene, emitters & controls

### 3.1 Cleaning & protection
- [ ] Assess pipework (steel/galv? → **do not** powerflush; re-pipe recommended)
- [ ] Clean: powerflush **or** chemical clean & inhibit
- [ ] Protect: magnetic filter (e.g., TF1 Omega) + inhibitor dose
- [ ] Evidence: TDS/clarity photos; flush report

### 3.2 Radiators & pipework
- [ ] Replace/add radiators (sizes/outputs)
- [ ] Fit **TRVs** & lockshields; ensure bypass path or auto-bypass
- [ ] **Balance** on completion; record ΔT/lockshield positions
- [ ] Cap redundant pipework; note microbore/one-pipe constraints

### 3.3 Controls & zoning
- **If Combi**
  - [ ] Single-zone room stat (load compensation preferred) / Hive Mini
  <!-- rule: hive_or_smart = true -->
- **If System/Regular with cylinder**
  - [ ] **S-plan** (preferred) or **Y-plan**; new wiring centre if needed
  - [ ] Cylinder stat/probe; independent CH/DHW time & temperature control
  <!-- rule: hive_or_smart = true -->

---

## 4) Delivery & office notes
- [ ] Preferred AM / Preferred PM
- [ ] Access: large vehicle suitable / restricted
- [ ] Deliver to garage / to room within property
- [ ] Call ahead on arrival
- [ ] Double-handed lift / Stairs – no lift
- [ ] what3words: _______________________________
  <!-- w3w:write_to = ["Delivery notes","Office notes"] -->

- **Office**
  - [ ] Direct labour required
  - [ ] Specialist works: asbestos removal / specialist builder / scaffolding
  - [ ] Assistance: double-handed required
  - [ ] what3words: use same as delivery
  <!-- w3w:mirror_delivery = true -->

---

## 5) Customer actions
- [ ] Clear working areas
- [ ] Gain permission where required (listed/flats/management)
- [ ] Ensure animals are kept safely
- [ ] Remove cupboard / Rebuild cupboard
- [ ] Remove old flue & weather seal
- [ ] Supply specified items

---

## 6) External hazards & restrictions
### Hazards
- [ ] Asbestos suspected
- [ ] Fragile roof tiles/material
- [ ] Flood risk / standing water
- [ ] Wasps / Bees nesting
- [ ] Poor lighting / no power
- [ ] Dogs / other potentially dangerous animals

### Restrictions
- [ ] No loft access / Restricted clearances
- [ ] Parking limited / permit required / Working hours restricted
- [ ] Septic tank – not suitable for condensate
- [ ] Listed building – consent/permission required
- [ ] Flats – management permission required

---

## 7) Flue (new & making good)
- [ ] Make good: old balanced / fanned / roof terminal / brick up
- [ ] New hole (same wall / alternative wall) OR reuse hole (minor change)
- [ ] Orientation: horizontal / vertical
- [ ] Seal brickwork to flue / Vertical flashing kit / Flat-roof flashing by specialist
- [ ] Plume kit / Flue extension / Terminal guard
- [ ] Orientation: front aspect / rear aspect
- **Clearances & routing**
  - [ ] ≥300 mm from openings; ≥600 mm to facing surface/boundary
  - [ ] Voids: inspection hatches at every joint/change of direction
  - [ ] Fall ~26–50 mm per metre back to boiler
  - [ ] High-rise: fire-rated flue only
  <!-- rule: flue_work = true -->

---

# Auto Arse-Covers (generated by rules)

> Your app should add the following **only when the matching rule comments above evaluate true**.

- **If `open_to_sealed`** (e.g., Regular open-vented → Combi/System/Unvented):  
  - Sealing an old system may expose hidden leaks  
  - Existing radiators/valves may leak once pressurised  
  - Old vented pipework/joints not designed for pressure  
  - Pressure drops after installation may indicate existing weeps/hidden leaks  
  - Customer to monitor pressure during initial days of use

- **If `combi_selected`**:  
  - Combination boilers supply one outlet at a time — flow reduces with multiple use  
  - Hot water performance limited by incoming mains pressure & flow  
  - Shower pumps/power showers incompatible with combis — remove  
  - Hot water temperature varies slightly with flow rate

- **If `unvented_selected`**:  
  - Unvented discharge tested at installation only; G3 compliance applies  
  - T&P relief via tundish to a safe termination required  
  - Unvented/Mixergy cylinders require periodic servicing for safety

- **If `condensate_present`** (always for condensing boilers):  
  - External condensate requires insulation and correct fall; freezing risk remains  
  - External soakaway/soil stack used where suitable drainage exists  
  - Customer responsible for keeping condensate route clear and free-flowing

- **If `hive_or_smart`**:  
  - Controls installed to manufacturer’s instructions  
  - Hive can operate without Wi-Fi; app features require router power/connection  
  - No responsibility for internet connectivity or app integration issues  
  - Room thermostat location based on best judgement at survey

- **If `flue_work`**:  
  - Flue termination clearances checked at time of install; future obstructions not covered  
  - Brickwork/render made good to a reasonable standard (not decorative)  
  - Flue sealing/flashings are weatherproof only (not decorative)

- **Always include General**:  
  - All works carried out to Gas Safe and Building Regulations at time of install  
  - Manufacturer warranty subject to annual service  
  - No liability for pre-existing faults or unrelated plumbing issues  
  - Performance depends on existing system design and pipework
