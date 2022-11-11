# openVAG
a project towards open HW+SW for fully scanning &amp; programming Volkswagen group cars

# Roadmap
The "endgame" would be a database of 
* vendor/proprietary protocol specs (with any salts, hash generation, key verification logic etc.)
* database of available long (programming) codes, non-standard vendor specific codes, all accompanied by a detailed description
* simple SW tool to use *any* code with some cheap existing OBD2 tool (read: ELM327)
* (optionally) a simple open-HW implementation

To work towards the "endgame" stage, would need:
* research & gather existing published code/data
* start sniffing and discover protocol at some stage in the current (MS Windows) tools [ SW -> USB-driver -> USB -> HW tool (UART? -> CAN) -> OBD2 ]
* a legal way to "discover" the programming codes; 
e.g., existing Ross-Tech VCDS (VAGcom diagnostics system) HW + SW should contain all of the codes, most probably the whole of the codes is located in some .CAB files on the Windows SW side. These, if not immediately obvious how to directly extract, probably could be sniffed through SW or HW intervention when programming a real car and then re-testing those codes with the simple SW tool (WIP)

For comments, ideas, will to participate, contact me.
