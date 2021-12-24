# vibra-contracts
Smart contracts for Vibra ecosystem

escrow.sol webshop.sol

ItemType: DIGITAL, PHYSICAL
ItemStatus: AVAILABLE, IN_TRANSIT, SOLD, REMOVED

A user creates a webshop, and adds items to their shop. Each item will have an ItemType variable that lets us know if it’s DIGITAL or PHYSICAL.

If digital, simply send payment to the seller. If physical, create an escrow contract, and deposit the money. At that point, the items status will be updated to IN_TRANSIT, and the tracking number will be added to the item.



Once the buyer confirms they received the product, the escrow pays out and is closed. Then the Item status is updated to SOLD, and the owner is updated to the new owner.
