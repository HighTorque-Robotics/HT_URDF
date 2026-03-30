cmake_minimum_required(VERSION 2.8.3)

project(PiPlusPro_S_12L10A2G2H1W_ZedMini_260322)

find_package(catkin REQUIRED)

catkin_package()

find_package(roslaunch)

foreach(dir config launch meshes urdf)
	install(DIRECTORY ${dir}/
		DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/${dir})
endforeach(dir)
