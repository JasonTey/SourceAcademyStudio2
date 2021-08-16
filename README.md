// Type your program in here!


function biggie_size (small_combo) {
    return small_combo + 4;
}

function unbiggie_size (big_combo) {
    return big_combo - 4;
}

function is_biggie_size (combo) {
    return combo > 4 ? true:false;
}

function combo_price (combo) {
    const patty = 1.17;
    const upzise = 0.50;
    return combo > 4 ? ((combo-4) * patty) + upzise:combo*patty;
}

function empty_order(){
    return 0;
}

function add_to_order (order, combo){
    return (order*10) + combo;
}


function last_combo(order) {
    return order%10;
}

function other_combos (order) {
    return (order - last_combo(order))/10;
}

other_combos(1534);






