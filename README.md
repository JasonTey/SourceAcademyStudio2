// Type your program in here!

import {
    
    show,circle,rcross,sail,corner,nova,heart,pentagram,ribbon,square,beside,beside_frac,color,flip_horiz,
flip_vert,make_cross,overlay,overlay_frac,quarter_turn_left,quarter_turn_right,repeat_pattern,rotate,
scale,scale_independent,stack,stack_frac,stackn,translate
    
} from "rune";

function turn_upside_down (rune) {
return quarter_turn_right(quarter_turn_right(rune));
}


function quarter_turning_left (rune) {
return quarter_turn_right(turn_upside_down(rune));
}



function go_beside (rune1,rune2) {
return quarter_turn_left(stack(quarter_turn_right(rune1),quarter_turn_right (rune2)));
}

const my_quilt = stackn(5,quarter_turn_right(stackn(7,quarter_turn_left(heart))));

show(stack(beside(quarter_turn_right(heart) ,turn_upside_down(heart)),beside (heart,quarter_turn_left(heart))));


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






