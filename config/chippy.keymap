/*
 * Copyright (c) 2020 The ZMK Contributors
 *
 * SPDX-License-Identifier: MIT
 */

#include <behaviors.dtsi>
#include <dt-bindings/zmk/keys.h>
#include <dt-bindings/zmk/bt.h>

/ {
        keymap {
                compatible = "zmk,keymap";

                default_layer {
// -----------------------------------------------------------------------------------------
// |  TAB |  Q  |  W  |  E  |  R  |  T  |   |  Y  |  U   |  I  |  O  |  P  | BKSP |
// | LALT |  A  |  S  |  D  |  F  |  G  |   |  H  |  J   |  K  |  L  |  ;  |  '   |
// | SHFT |  Z  |  X  |  C  |  V  |  B  |   |  N  |  M   |  ,  |  .  |  /  | ESC  |
//                    | GUI | (LWR CTRL) | ENT |   | SPC | (RSE BKPS)  | ALT |
                        bindings = <
   &trans   &kp Q &kp W &kp E &kp R &kp T   &kp Y &kp U  &kp I     &kp O   &kp P    &trans
   &trans &kp A &kp S &kp D &kp F &kp G   &kp H &kp J  &kp K     &kp L   &kp SEMI &trans
   &trans &mt LSHFT Z &kp X &kp C &kp V &kp B   &kp N &lt 2 M  &kp COMMA &kp DOT &mt RSHFT FSLH &trans
                  &kp TAB &kp LCTRL &mt LGUI RET   &lt 1 SPACE &kp BSPC &kp RALT
                        >;
                };
                lower_layer {
// -----------------------------------------------------------------------------------------
// |  TAB |  1  |  2  |  3  |  4  |  5  |   |  6  |  7  |  8  |  9  |  0  | BKSP |
// | BTCLR| BT1 | BT2 | BT3 | BT4 | BT5 |   |     | LFT | DWN | UP  | RGT |      |
// | SHFT |     |     |     |     |     |   |     |     |     |     |     |      |
//                    | GUI |     | ENT |   | SPC |     | ALT |
                        bindings = <
   &trans   &trans      &kp N7       &kp N8   &kp N9     &kp N0          &kp HOME   &kp PG_DN   &kp PG_UP &kp END    &kp N0 &trans
   &trans    &trans      &kp N4       &kp N5   &kp N6     &trans         &kp LEFT &kp DOWN &kp UP &kp RIGHT &trans  &trans
   &trans &kp LSHFT   &kp N1       &kp N2   &kp N3     &trans         &bt BT_SEL 4   &bt BT_SEL 3   &bt BT_SEL 2 &bt BT_SEL 1  &bt BT_SEL 0 &bt BT_CLR
                                    &kp TAB    &kp LCTRL   &kp LSHFT      &kp SPACE  &kp BSPC   &kp RALT
                        >;
                };

                raise_layer {
// -----------------------------------------------------------------------------------------
// |  TAB | #     |  ;  |  (  |  )  |  "  |   |    |    |    |    |    |    |
// | CTRL | "|"   |  >  |  [{ | }]  |  :  |   |    |    |    |    |    |    |
// | SHFT | SHFT  |  %  |  -  |  _  |  =  |   |    |    |    |    |    |    |
//                    | GUI |     | ENT |   | SPC |     | ALT |
                        bindings = <
   &kp  TAB  &kp HASH    &kp SEMICOLON &kp LPAR    &kp RPAR    &kp DQT          &kp K_PLAY_PAUSE &kp K_STOP  &kp K_VOL_UP &kp K_VOL_DOWN &kp RPAR &kp BSPC
   &kp LCTRL &kp PIPE    &kp GT        &kp LBKT    &kp LBRC    &kp COLON           &trans &trans &kp GRAVE  &kp BSLH &trans &trans
   &kp LSHFT &kp LSHFT   &kp PERCENT   &kp MINUS   &kp UNDER   &kp EQUAL        &trans &trans  &trans &trans &kp RSHFT &trans
                             &kp LGUI &trans   &kp LSHFT                        &kp SPACE   &kp BSPC    &kp RALT
                        >;
                };
        };
};
