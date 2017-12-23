cmake_minimum_required(VERSION 3.6)
project (apoc C)
set(CMAKE_CXX_STANDARD 11)

set(SOURCE_FILES
    src/act.comm.c
    src/act.informative.c
    src/act.item.c
    src/act.movement.c
    src/act.offensive.c
    src/act.other.c
    src/act.social.c
    src/act.wizard.c
    src/aedit.c
    src/alias.c
    src/ban.c
    src/boards.c
    src/bsd-snprintf.c
    src/castle.c
    src/cedit.c
    src/class.c
    src/comm.c
    src/config.c
    src/constants.c
    src/db.c
    src/fight.c
    src/genmob.c
    src/genobj.c
    src/genolc.c
    src/genshp.c
    src/genwld.c
    src/genzon.c
    src/graph.c
    src/handler.c
    src/house.c
    src/improved-edit.c
    src/interpreter.c
    src/limits.c
    src/magic.c
    src/mail.c
    src/medit.c
    src/mobact.c
    src/modify.c
    src/oasis.c
    src/oasis_copy.c
    src/oasis_delete.c
    src/oasis_list.c
    src/objsave.c
    src/oedit.c
    src/olc.c
    src/random.c
    src/redit.c
    src/sedit.c
    src/shop.c
    src/spec_assign.c
    src/spec_procs.c
    src/spell_parser.c
    src/spells.c
    src/tedit.c
    src/utils.c
    src/weather.c
    src/zedit.c
)
add_executable(circle ${SOURCE_FILES})
target_link_libraries(circle crypt)
