# CMakeList.txt : fichier projet CMake de niveau supérieur, effectuez une configuration globale
# et incluez les sous-projets ici.
#
cmake_minimum_required (VERSION 3.8)

# Solution
project ("SAE921-GRP4100-Box2D")
message("SOLUTION/PROJECT CMAKING " ${CMAKE_PROJECT_NAME})

include_directories(../_Utilities/include/)
file(GLOB_RECURSE PLATFORMER_SRC ../_Utilities/src/*.cpp)

# Each sub-project
set(EXECUTABLE_CUSTOM_NAME "00-Starter")
add_subdirectory ("00-Starter")
# Each sub-project
set(EXECUTABLE_CUSTOM_NAME "0-Formative-Arkanoid")
add_subdirectory ("0-Formative-Arkanoid")
# Each sub-project
set(EXECUTABLE_CUSTOM_NAME "0-Formative-Starship")
add_subdirectory ("0-Formative-Starship")
# Each sub-project
set(EXECUTABLE_CUSTOM_NAME "01-Gravity")
add_subdirectory ("01-Gravity")
# Each sub-project
set(EXECUTABLE_CUSTOM_NAME "02-Bouncing")
add_subdirectory ("02-Bouncing")
# Each sub-project
set(EXECUTABLE_CUSTOM_NAME "02-BouncingAndCollsions")
add_subdirectory ("02-BouncingAndCollsions")
# Each sub-project
set(EXECUTABLE_CUSTOM_NAME "03-BouncingAdvanced")
add_subdirectory ("03-BouncingAdvanced")
# Each sub-project
set(EXECUTABLE_CUSTOM_NAME "04-ZeroGravity")
add_subdirectory ("04-ZeroGravity")
# Each sub-project
set(EXECUTABLE_CUSTOM_NAME "05-SpriteMovement")
add_subdirectory ("05-SpriteMovement")
