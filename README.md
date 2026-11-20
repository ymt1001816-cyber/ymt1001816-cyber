# MeiYu "Cindy" Kuo

**Design Verification · RTL Design · DFT · Physical Design**

I build small chips end to end and don't trust one check: every chip design here is verified by simulation, a reference model **and** formal proof, then taken to a signed-off layout.
M.S. Semiconductor Engineering, Northeastern University (May 2028) · Bay Area, CA.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/cindy-kuo-bba758354/) ![Open to](https://img.shields.io/badge/Open%20to-Summer%202027%20internships-2ea44f) ![Focus](https://img.shields.io/badge/Focus-DV%20%C2%B7%20RTL%20%C2%B7%20DFT-0F766E)

**Keywords:** `Verilog` `SystemVerilog` `UVM` `SVA` `cocotb` `Formal (SymbiYosys)` `Conformal LEC` `CDC` `Scan / ATPG` `MBIST` `Genus` `Innovus` `OpenROAD` `STA` `Virtuoso` `Python` `TCL` `CI/CD`

---

### Featured projects

<table>
<tr>
<td width="50%" valign="top">
<img src="assets/cache.svg" width="72" alt=""><br>
<b><a href="https://github.com/ymt1001816-cyber/cache-rtl-to-signoff">1 KB Cache: RTL to Signoff</a></b><br>
45 nm cache taken from Verilog to a DRC-clean, LVS-correct layout, then made testable and low-power.
<p><b>UVM 100% functional coverage · 4/4 planted bugs caught · LEC proves RTL = netlist = layout · clock gating cuts power 86% while scan coverage stays at 99.84%</b></p>
<code>UVM</code> <code>cocotb</code> <code>formal</code> <code>Innovus</code> <code>OpenROAD</code> <code>scan/ATPG</code> <code>MBIST</code>
</td>
<td width="50%" valign="top">
<img src="assets/fifo.svg" width="72" alt=""><br>
<b><a href="https://github.com/ymt1001816-cyber/async-fifo-cdc">Async FIFO: the CDC bug simulation can't see</a></b><br>
Dual-clock FIFO checked with cocotb and with formal using a metastability model.
<p><b>Binary-pointer bug passes every simulation, formal catches it in 11 steps · Gray-code version proven for any clock ratio</b></p>
<code>CDC</code> <code>SymbiYosys</code> <code>k-induction</code> <code>cocotb</code>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<img src="assets/sram.svg" width="72" alt=""><br>
<b><a href="https://github.com/ymt1001816-cyber/sram-bisr">SRAM Built-In Self-Repair</a></b><br>
Programmable March MBIST finds bad cells, redundancy analysis picks spares, the address path remaps them.
<p><b>2 spare rows + 2 spare columns repair 99.8% of line faults vs 66% with rows only · fault injection shows what March C- misses</b></p>
<code>MBIST</code> <code>BIRA</code> <code>DFT</code> <code>formal equivalence</code>
</td>
<td width="50%" valign="top">
<img src="assets/ivchar.svg" width="72" alt=""><br>
<b><a href="https://github.com/ymt1001816-cyber/ivchar">ivchar: MOSFET I-V characterization</a></b><br>
Python tool that drives a B1500A or SCPI SMU, extracts Vth / SS / DIBL and writes a yield report.
<p><b>Tracks BSIM corner Vth shifts within 3 mV · 83 tests in CI · example data is simulated</b></p>
<code>Python</code> <code>PyVISA</code> <code>pandas</code> <code>device physics</code>
</td>
</tr>
</table>

---

### Why these projects
- **Bugs that one method misses.** Each repo shows a bug that slipped past the first check and what caught it: signoff, formal, or a reference model.
- **Reproducible.** Every repo runs its full regression in GitHub Actions on every push; the open-source layout flow runs there too.
- **Design for test, not after.** Low-power and DFT were built together, so clock gating didn't cost scan coverage.

<sub>Looking for Summer 2027 internships in design verification, RTL design or DFT. Happy to walk through any of these projects.</sub>
