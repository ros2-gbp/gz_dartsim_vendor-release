^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package gz_dartsim_vendor
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

0.1.3 (2026-04-20)
------------------
* Merge pull request `#9 <https://github.com/gazebo-release/gz_dartsim_vendor/issues/9>`_ from gazebo-release/jrivero/bump_6_16
  Bump dart vendor in rolling to 6.16.6
* Bump DART version to 6.16.6
* Update patch
* Contributors: Jose Luis Rivero

0.1.2 (2024-11-26)
------------------
* Add check for system installed dartsim (`#6 <https://github.com/gazebo-release/gazebo_dartsim_vendor/issues/6>`_)
  * Check for system installed dart first.
  * Update dart version and add extra debug message
  * Add relaxed version matching when requested
  ---------
  Co-authored-by: Rhys Mainwaring <rhys.mainwaring@me.com>
* Contributors: Øystein Sture

0.1.1 (2024-06-25)
------------------
* Switch to using the liboctomap-dev key for a dependency. (`#5 <https://github.com/gazebo-release/gazebo_dartsim_vendor/issues/5>`_)
  This is now available in rosdep.
* Contributors: Chris Lalancette

0.1.0 (2024-04-25)
------------------

0.0.2 (2024-04-02)
------------------
* Add dependency on fmt, patch pkgconfig installation
* Change version to 0.0.1
* Fix linter (`#3 <https://github.com/gazebo-release/gazebo_dartsim_vendor/issues/3>`_)
* Remove Octomap (`#2 <https://github.com/gazebo-release/gazebo_dartsim_vendor/issues/2>`_)
  Octomap is an optional dependency. There seems to be an issue resolving
  this key on the ROS buildfarm, so disabling it for now.
  This also removes `DART_BUILD_OSG` cmake flag, which does not exist in 6.13.2
* Add README (`#1 <https://github.com/gazebo-release/gazebo_dartsim_vendor/issues/1>`_)
* Rename to gz_dartsim_vendor
* Add license and contributing files
* Change name and update version
* Remove optional packages
* Initial import
* Contributors: Addisu Z. Taddese
