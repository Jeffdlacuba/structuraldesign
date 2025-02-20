This example %% ================================================================
%% Interaction Diagram for Reinforced Concrete Wall - Wall C
%% ================================================================
%% Purpose of this Code
% This script generates an interaction diagram for a reinforced concrete wall section.
% The interaction diagram is a graphical representation of the axial force vs. bending moment
% relationship, which helps in understanding the structural capacity of the wall under
% combined loading conditions.
%% ================================================================
%% How it Works
% - The script first defines the material properties of concrete and reinforcement steel.
% - The geometric properties of the wall section are then specified.
% - The reinforcement distribution is input, and its strain state is evaluated for different
%   positions of the neutral axis.
% - Based on strain compatibility and equilibrium equations, the axial force and moment
%   capacities are computed for both positive (tension) and negative (compression) loading.
% - The factored capacities are calculated based on reduction factors.
% - The interaction diagram is plotted to visualize the axial-moment capacity envelope.
%% ================================================================
%% Why it is Necessary
% - Understanding the interaction between axial force and bending moment is crucial for
defining safe design limits for reinforced concrete walls in structural engineering.
% - This analysis ensures compliance with design codes such as ACI-318 by verifying
%   that the structural component can withstand expected loads without failure.
%% ================================================================
%% Inputs
% - Concrete compressive strength (f'c)
% - Steel yield strength (fy)
% - Section geometry (widths and heights of different segments)
% - Reinforcement layout and properties
% - Ultimate strain conditions
%% ================================================================
%% Outputs
% - Interaction diagram displaying nominal and factored axial force vs. moment capacity.
% - Maximum axial force and bending moment capacities.
%% ================================================================
%% Source Model
% Calderon, V. H. (2021). "Feasibility of protecting with seismic isolation a limited-ductility-wall social housing."
% (In Spanish) Pontifical Catholic University of Peru Digital Repository.
% Available at: https://tesis.pucp.edu.pe/items/033969e7-0b01-494f-ac01-6d2167bd67d4
%% ================================================================
%% Authors
% - Originally created by: Victor Calderon (May 2015)
% - Optimized by: Jefferson De la Cuba (February 2025)
%% ================================================================

clear
close all
clc

