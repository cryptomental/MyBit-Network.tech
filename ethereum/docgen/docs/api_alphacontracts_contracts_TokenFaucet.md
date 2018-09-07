---
id: alphacontracts_contracts_TokenFaucet
title: TokenFaucet
---

<div class="contract-doc"><div class="contract"><h2 class="contract-header"><span class="contract-kind">contract</span> TokenFaucet</h2><div class="source">Source: <a href="https://github.com/MyBitFoundation/MyBit-Network.tech//blob/v0.0.0/contracts/alphacontracts/contracts/TokenFaucet.sol" target="_blank">alphacontracts/contracts/TokenFaucet.sol</a></div></div><div class="index"><h2>Index</h2><ul><li><a href="alphacontracts_contracts_TokenFaucet.html#LogEthDeposited">LogEthDeposited</a></li><li><a href="alphacontracts_contracts_TokenFaucet.html#LogEthWithdraw">LogEthWithdraw</a></li><li><a href="alphacontracts_contracts_TokenFaucet.html#LogMYBDeposited">LogMYBDeposited</a></li><li><a href="alphacontracts_contracts_TokenFaucet.html#LogNewUser">LogNewUser</a></li><li><a href="alphacontracts_contracts_TokenFaucet.html#LogWithdraw">LogWithdraw</a></li><li><a href="alphacontracts_contracts_TokenFaucet.html#anyOwner">anyOwner</a></li><li><a href="alphacontracts_contracts_TokenFaucet.html#basicVerification">basicVerification</a></li><li><a href="alphacontracts_contracts_TokenFaucet.html#changePass">changePass</a></li><li><a href="alphacontracts_contracts_TokenFaucet.html#depositWEI">depositWEI</a></li><li><a href="alphacontracts_contracts_TokenFaucet.html#">fallback</a></li><li><a href="alphacontracts_contracts_TokenFaucet.html#receiveApproval">receiveApproval</a></li><li><a href="alphacontracts_contracts_TokenFaucet.html#withdraw">withdraw</a></li></ul></div><div class="reference"><h2>Reference</h2><div class="events"><h3>Events</h3><ul><li><div class="item event"><span id="LogEthDeposited" class="anchor-marker"></span><h4 class="name">LogEthDeposited</h4><div class="body"><code class="signature">event <strong>LogEthDeposited</strong><span>(address _depositer, uint _amountWEI) </span></code><hr/><dl><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>_depositer</code> - address</div><div><code>_amountWEI</code> - uint</div></dd></dl></div></div></li><li><div class="item event"><span id="LogEthWithdraw" class="anchor-marker"></span><h4 class="name">LogEthWithdraw</h4><div class="body"><code class="signature">event <strong>LogEthWithdraw</strong><span>(address _withdrawer, uint _amountWEI) </span></code><hr/><dl><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>_withdrawer</code> - address</div><div><code>_amountWEI</code> - uint</div></dd></dl></div></div></li><li><div class="item event"><span id="LogMYBDeposited" class="anchor-marker"></span><h4 class="name">LogMYBDeposited</h4><div class="body"><code class="signature">event <strong>LogMYBDeposited</strong><span>(address _depositer, uint _amount, bytes _data) </span></code><hr/><dl><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>_depositer</code> - address</div><div><code>_amount</code> - uint</div><div><code>_data</code> - bytes</div></dd></dl></div></div></li><li><div class="item event"><span id="LogNewUser" class="anchor-marker"></span><h4 class="name">LogNewUser</h4><div class="body"><code class="signature">event <strong>LogNewUser</strong><span>(address _user) </span></code><hr/><dl><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>_user</code> - address</div></dd></dl></div></div></li><li><div class="item event"><span id="LogWithdraw" class="anchor-marker"></span><h4 class="name">LogWithdraw</h4><div class="body"><code class="signature">event <strong>LogWithdraw</strong><span>(address _sender, uint _amountMYB, uint _amountWEI) </span></code><hr/><dl><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>_sender</code> - address</div><div><code>_amountMYB</code> - uint</div><div><code>_amountWEI</code> - uint</div></dd></dl></div></div></li></ul></div><div class="modifiers"><h3>Modifiers</h3><ul><li><div class="item modifier"><span id="anyOwner" class="anchor-marker"></span><h4 class="name">anyOwner</h4><div class="body"><code class="signature">modifier <strong>anyOwner</strong><span>() </span></code><hr/></div></div></li><li><div class="item modifier"><span id="basicVerification" class="anchor-marker"></span><h4 class="name">basicVerification</h4><div class="body"><code class="signature">modifier <strong>basicVerification</strong><span>(uint _newAccessLevel) </span></code><hr/><dl><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>_newAccessLevel</code> - uint</div></dd></dl></div></div></li></ul></div><div class="functions"><h3>Functions</h3><ul><li><div class="item function"><span id="changePass" class="anchor-marker"></span><h4 class="name">changePass</h4><div class="body"><code class="signature">function <strong>changePass</strong><span>(bytes32 _newPass) </span><span>external </span><span>returns  (bool) </span></code><hr/><dl><dt><span class="label-modifiers">Modifiers:</span></dt><dd><a href="alphacontracts_contracts_TokenFaucet.html#anyOwner">anyOwner </a></dd><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>_newPass</code> - bytes32</div></dd><dt><span class="label-return">Returns:</span></dt><dd>bool</dd></dl></div></div></li><li><div class="item function"><span id="depositWEI" class="anchor-marker"></span><h4 class="name">depositWEI</h4><div class="body"><code class="signature">function <strong>depositWEI</strong><span>() </span><span>external </span><span>payable </span></code><hr/></div></div></li><li><div class="item function"><span id="fallback" class="anchor-marker"></span><h4 class="name">fallback</h4><div class="body"><code class="signature">function <strong></strong><span>(address _database, address _mybTokenAddress, bytes32 _accessPass) </span><span>public </span></code><hr/><dl><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>_database</code> - address</div><div><code>_mybTokenAddress</code> - address</div><div><code>_accessPass</code> - bytes32</div></dd></dl></div></div></li><li><div class="item function"><span id="receiveApproval" class="anchor-marker"></span><h4 class="name">receiveApproval</h4><div class="body"><code class="signature">function <strong>receiveApproval</strong><span>(address _from, uint _amount, address _mybToken, bytes _data) </span><span>external </span></code><hr/><dl><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>_from</code> - address</div><div><code>_amount</code> - uint</div><div><code>_mybToken</code> - address</div><div><code>_data</code> - bytes</div></dd></dl></div></div></li><li><div class="item function"><span id="withdraw" class="anchor-marker"></span><h4 class="name">withdraw</h4><div class="body"><code class="signature">function <strong>withdraw</strong><span>(string _pass) </span><span>external </span></code><hr/><dl><dt><span class="label-parameters">Parameters:</span></dt><dd><div><code>_pass</code> - string</div></dd></dl></div></div></li></ul></div></div></div>