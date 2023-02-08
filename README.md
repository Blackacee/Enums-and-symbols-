# Enums-and-symbols-

// Simple symbol
const newSymbol = Symbol();
typeof newSymbol === 'symbol' // true
// A symbol with a label
const anotherSymbol = Symbol("label");
// Each symbol is unique
const yetAnotherSymbol = Symbol("label");
yetAnotherSymbol === anotherSymbol; // false
const Regnum_Animale = Symbol();
const Regnum_Vegetabile = Symbol();
const Regnum_Lapideum = Symbol();
function describe(kingdom) {
 switch(kingdom) {
 case Regnum_Animale:
 return "Animal kingdom";
 case Regnum_Vegetabile:
 return "Vegetable kingdom";
 case Regnum_Lapideum:
 return "Mineral kingdom";
 }
}
describe(Regnum_Vegetabile);
// Vegetable kingdom
