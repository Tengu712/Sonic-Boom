# Sonic Boom Compiled Music Binary Data Structure

## Music Block

1. max parts count (u8)
1. operators count (u8)
1. operators (Operator Block * operators count)
1. algorythms count (u8)
1. algorythms (Algorythm Block * algorythms count)
1. songs count (u32)
1. songs (Song Block * songs count)

## Operator Block

1. attack (u8)
1. decay (u8)
1. sustain (u8)
1. release (u8)
1. total (u8)
1. multiple (u8)

## Algorythm Block

1. commands count (u8)
1. commands (Algorythm Command Block * commands count)

## Algorythm Command Block

1. command id (u8)
1. operator id (u8)

## Song Block

1. parts count (u8)
1. parts (Part Block * parts count)

## Part Block

1. part id (u8)
1. algorythm id (u8)
1. notes count (u32)
1. notes (Note Block * notes count)

## Note Block

1. time (u32)
1. gate (u32)
1. amplitude (f32)
1. frequency (f32)
