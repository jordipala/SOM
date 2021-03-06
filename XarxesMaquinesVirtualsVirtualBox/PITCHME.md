Configuració de la xarxa a les màquines virtuals
================================================

[Veure Teoria](https://jrodr236.github.io/SOM/XarxaMaquinesVirtuals.html)

---

## Hardware virtual
<img src="https://i.pinimg.com/originals/51/0d/fd/510dfd4b05143f8c54ba1a2a876c4cd7.jpg" height="500px">

+++

<img src="http://www.szedup.com/wp-content/uploads/2018/05/EP-N1581-3.jpg" height="500px">

---

## Modes de Xarxa

* No connectat
* NAT
* Xarxa NAT
* Adaptador pont
* Xarxa interna
* Adaptador de només amfitrió

+++

### No connectat
<img src="https://www.tutorialspoint.com/communication_technologies/images/ethernet_card.jpg" height="500px">

+++

### NAT

![](https://cdn.app.compendium.com/uploads/user/e7c690e8-6ff9-102a-ac6d-e4aebca50425/f2e3e7b6-c53b-4457-85e9-49625315791a/Image/90093dc07a2e9cb7d93bf7a3fa8f8c19/nat.png)

Les VM estan desconnectades entre si.

+++

### Xarxa NAT

![](https://cdn.app.compendium.com/uploads/user/e7c690e8-6ff9-102a-ac6d-e4aebca50425/f2e3e7b6-c53b-4457-85e9-49625315791a/Image/04856a6937656d8c2a2e0dd30855f3ba/nat_port_forward.png)

Les VM estan connectades entre si

*No confondre amb* ***NAT***

+++

### Adaptador pont

![](https://cdn.app.compendium.com/uploads/user/e7c690e8-6ff9-102a-ac6d-e4aebca50425/f2e3e7b6-c53b-4457-85e9-49625315791a/Image/5e1da37f793c380abd4375ff64b21c70/bridged.png)

+++

### Xarxa interna

![](https://cdn.app.compendium.com/uploads/user/e7c690e8-6ff9-102a-ac6d-e4aebca50425/f2e3e7b6-c53b-4457-85e9-49625315791a/Image/d16091a2abef68694625196dd18f588a/internal.png)

+++

### Adaptador de només amfitrió

![](https://cdn.app.compendium.com/uploads/user/e7c690e8-6ff9-102a-ac6d-e4aebca50425/f2e3e7b6-c53b-4457-85e9-49625315791a/Image/1ae51906a03cffa842010fd6d6937c61/host_only.png)

+++

### Mòdul genèric

Poc utilitzat.

+++

### Resum

&nbsp;|VM ↔ Host|VM1 ↔ VM2|VM → Internet|VM ← Internet
---------|:---------:|:-------------:|:-------------:|:----:
Host-only|+|+|–|–
Internal|–|+|–|–

+++

&nbsp;|VM ↔ Host|VM1 ↔ VM2|VM → Internet|VM ← Internet
---------|:---------:|:-------------:|:-------------:|:----:
Bridged|+|	+|	+|	+
NAT|	–|	–|	+|	Port forwarding
NAT Network|	–|	+|	+|	Port forwarding
