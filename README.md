# fleet-teams-gitops

This action applies the latest team configuration files to Fleet.

Example usage
steps:
  - name: Apply configuration profiles and updates
    uses: fleetdm/fleet-mdm-gitops
    with:
      FLEET_API_TOKEN: ${{ secrets.FLEET_API_TOKEN }}
      FLEET_URL: ${{ secrets.FLEET_URL }}
      TEAM_DIRECTORY: mdm_profiles
  