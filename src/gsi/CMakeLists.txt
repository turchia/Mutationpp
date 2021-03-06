#
# Copyright 2014-2018 von Karman Institute for Fluid Dynamics (VKI)
#
# This file is part of MUlticomponent Thermodynamic And Transport
# properties for IONized gases in C++ (Mutation++) software package.
#
# Mutation++ is free software: you can redistribute it and/or modify
# it under the terms of the GNU Lesser General Public License as
# published by the Free Software Foundation, either version 3 of the
# License, or (at your option) any later version.
#
# Mutation++ is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU Lesser General Public License for more details.
#
# You should have received a copy of the GNU Lesser General Public
# License along with Mutation++.  If not, see
# <http://www.gnu.org/licenses/>.
#

cmake_minimum_required(VERSION 2.6)

add_sources(mutation++
    DiffusionVelocityCalculator.cpp
    GasSurfaceInteraction.cpp
    GSIReactionAblation.cpp
    GSIReactionCatalysis.cpp
    GSIRateLawGammaConst.cpp
    GSIRateLawGammaT.cpp
    GSIRateLawSublimation.cpp
    GSIRateManagerGamma.cpp
    GSIStoichiometryManager.cpp
    MassBlowingRateAblation.cpp
    MassBlowingRateNull.cpp
    SurfaceBalanceSolverMass.cpp
    SurfacePropertiesNull.cpp
    WallState.cpp
    WallProductionTermsEmpty.cpp
    WallProductionSurfaceChemistry.cpp
    WallProductionPyrolysis.cpp
)

install(FILES DiffusionVelocityCalculator.h DESTINATION include/mutation++)
install(FILES GasSurfaceInteraction.h DESTINATION include/mutation++)
install(FILES GSIRateLaw.h DESTINATION include/mutation++)
install(FILES GSIRateManager.h DESTINATION include/mutation++)
install(FILES GSIReaction.h DESTINATION include/mutation++)
install(FILES GSIStoichiometryManager.h DESTINATION include/mutation++)
install(FILES MassBlowingRate.h DESTINATION include/mutation++)
install(FILES SurfaceBalanceSolver.h DESTINATION include/mutation++)
install(FILES SurfaceProperties.h DESTINATION include/mutation++)
install(FILES WallProductionTerms.h DESTINATION include/mutation++)
install(FILES WallState.h DESTINATION include/mutation++)
