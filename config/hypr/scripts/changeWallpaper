#!/bin/bash

DIR=$HOME/Pictures/wallpapers/
PICS=($(ls ${DIR}))

RANDOMPICS=${PICS[ $RANDOM % ${#PICS[@]} ]}

if [[ $(pidof swaybg) ]]; then
  pkill swaybg
fi

swaybg -m fill -i ${DIR}/${RANDOMPICS}
## notify-send "${RANDOMPICS}"
