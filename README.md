const z = 25 - (4 + 2) * 3;

z < 10 ? "small" : "big";

x && y stands for x ? y : false
z < 10 && z > -1 ? "z is within 0-9" : "z is outside 0-9";

x || y stands for x ? true : y
z >= 10 || z < 0 ? "z is outside 0-9" : "z is within 0-9";

// Question 1

// function biggie_size(x){
//     return x === 1 
//     ? 5
//     : x === 2
//     ? 6
//     : x === 3
//     ? 7
//     : x === 4
//     ? 8
//     : false;
// }

function biggie_size (small_combo) { return small_combo + 4; }

function unbiggie_size (big_combo) { return big_combo - 4; }

function is_biggie_size (combo) {
    return combo > 4;
}

function combo_price(order) {
    return order > 4 
           ? (order - 4) * 1.17 + 0.5 
           : order * 1.17;
}

function empty_order(){
    return 0;

}

function add_to_order(x,y){
    return x * 10 + y;
}



function last_combo(order) { 
    return order % 10; 
    
}

function other_combos(order){
    // return order / 10 - last_combo(order) / 10 ;
    return math_floor(order / 10);
}

math_floor(-2.5);

math_trunc(-2.5);

// other_combos(321);


    
    
    
    





